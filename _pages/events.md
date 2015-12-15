---
layout: home
description: "读书活动列表"
permalink: /events/
---

<section id="services">
    <div class="uk-container uk-container-center">
        <div class="uk-grid">
            <div class="uk-width-1-1 uk-overflow-container">
                <h2 class="service-heading uk-text-center">分享的书目</h2>
                    <table class="uk-table uk-table-hover uk-table-striped table-bordered">
                        <thead>
                            <tr>
                                <th>  </th>
                                <th> 日期 </th>
                                <th> 主讲人 </th>
                                <th> 书名 </th>
                                <th> 作者 </th>
                                <th> 类别 </th>
                            </tr>
                        </thead>

                        <tbody>
                            {% for book in site.data.book_list %}
                            <tr>
                                <td> {{ book.seq }} </td>
                                <td> {{ book.date }} </td>
                                <td> {{ book.speaker }} </td>
                                <td> {{ book.bookname }} </td>
                                <td> {{ book.author }} </td>
                                <td> {{ book.category }} </td>
                            </tr>
                            {% endfor %}
                        </tbody>
                    </table>
            </div>
        </div>
    </div>
</section>

