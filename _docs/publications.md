---
title: Công bố khoa học
permalink: /docs/publications/
---

##### Danh sách các công bố khoa học có sử dụng chùm tia từ máy gia tốc HUS Pelletron.

<div class="table-2">
	<table width="100%">
		<thead>
			<tr>
				<th align="left">STT</th>
				<th align="left">Tiêu đề</th>
				<th align="left">Tác giả</th>
				<th align="left">Tạp chí</th>
				<th align="left">Quyển; Số; Trang</th>
				<th align="left">Năm</th>
				<th align="left">Nhà xuất bản</th>
			</tr>
		</thead>
		<tbody id="results"></tbody>
	</table>
</div>

<script>
	fetch("/assets/publications_database.xml")
	.then(response => response.text())
	.then((data) => {
		let parser = new DOMParser(),
		xml = parser.parseFromString(data,"text/xml");
		var no = xml.getElementsByTagName('no');
		var title = xml.getElementsByTagName('title');
		var author = xml.getElementsByTagName('author');
		var journal = xml.getElementsByTagName('journal');
		var volumne = xml.getElementsByTagName('volumne');
		var number = xml.getElementsByTagName('number');
		var page = xml.getElementsByTagName('page');
		var year = xml.getElementsByTagName('year');
		var publisher = xml.getElementsByTagName('publisher');
		for (i = 0; i < no.length; i++) {
			no_i = no[i].childNodes[0].nodeValue;
			title_i = title[i].childNodes[0].nodeValue;
			author_i = author[i].childNodes[0].nodeValue;
			journal_i = journal[i].childNodes[0].nodeValue;
			volumne_i = volumne[i].childNodes[0].nodeValue;
			number_i = number[i].childNodes[0].nodeValue;
			page_i = page[i].childNodes[0].nodeValue;
			year_i = year[i].childNodes[0].nodeValue;
			publisher_i = publisher[i].childNodes[0].nodeValue;
			const row = `<tr>
						<td align="left">${no_i}</td>
						<td align="left">${title_i}</td>
						<td align="left">${author_i}</td>
						<td align="left">${journal_i}</td>
						<td align="left">${volumne_i}; ${number_i}; ${page_i}</td>
						<td align="left">${year_i}</td>
						<td align="left">${publisher_i}</td>
						</tr>`;
			const results = document.querySelector("#results");
			results.insertAdjacentHTML("beforeend",row);
		};
	});
</script>

