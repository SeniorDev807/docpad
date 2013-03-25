---
title: Writing
layout: default
tags: ['writing','gwen bell']
pageOrder: 6
---

.container.container-main
	.row
		.span4
			nav.linklist
				each doc in getCollection('posts').toJSON()
					p
						span= doc.date.toShortDateString()
						| |&nbsp;
						a(href=doc.url)= doc.title

		.span8
			img(src='/writing-in-berlin.jpg')