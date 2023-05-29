---
layout: "../../layouts/genericMarkdownFile.astro"
title: "Back End Lesson 5.2: Calling REST APIs with Fetch"
description: "imported from WordPress,Back End Lesson 5.2: Calling REST APIs with Fetch"
---

# Back End Lesson 5.2: Calling REST APIs with Fetch

Welcome to Lesson 5.2 of the Ruby on Rails Back End Class. In the previous lesson, you created a REST API in Rails. In this lesson, you will learn how to call that REST API from a web page that is hosted in Rails.

This lesson is primarily about JavaScript. If you do not have a background in JavaScript, it will be difficult for you to complete the lesson. The main JavaScript capabilities to be exercised in this lesson are (a) manipulation of, and interaction with, the web page DOM, and (b) retrieval of data using the JavaScript fetch API.

## Curriculum

This is your curriculum for Lesson 5.2:  
\***\*5.2.1[ Calling REST with Fetch](https://learn.codethedream.org/rails-calling-rest-with-fetch/)**

## Assignments

You continue to work on the same repository that was used for the previous lesson.

In addition to the above assignment, you will need to start thinking about what project you will like to build for your final project. The rubric for the final project is located here: **<https://learn.codethedream.org/back-end-2-final-project/>** Read through that page, come up with your idea for the final project that meets the requirements, and submit your plan using the **[l](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[a](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[s](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[t](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[ ](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[s](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[e](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[v](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[e](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[r](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[a](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[l](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[ ](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[q](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[u](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[e](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[s](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[t](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[i](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[o](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[n](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[s](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[ ](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[o](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[n](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[ ](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[y](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[o](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[u](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[r](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[ ](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[u](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[s](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[u](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[a](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[l](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[ ](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[H](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[o](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[m](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[e](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[w](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[o](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[r](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[k](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[ ](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[A](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[s](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[s](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[i](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[g](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[n](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[m](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[e](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[n](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[t](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[ ](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[S](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[u](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[b](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[m](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[i](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[s](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[s](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[i](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[o](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[n](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[ ](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[F](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[o](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[r](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)[m](https://airtable.com/shrBpqHbS6wgInoF9?prefill%5FLessons=Ruby%20on%20Rails%3A%20Lesson%205.2%20-%20Calling%20the%20API%20using%20AJAX)**. A mentor of the Ruby on Rails class will review your proposal and will communicate with you via Slack to let you know if you can begin your work or if your plan needs revisions before you can begin. Please contact the Class Coordinator if you have any questions.

Your mindset curriculum assignment can be found **[here](https://learn.codethedream.org/mindset-curriculum-design-part-1/)**.