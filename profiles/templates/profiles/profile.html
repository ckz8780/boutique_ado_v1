{% extends "base.html" %}
{% load static %}

{% block extra_css %}
    <link rel="stylesheet" href="{% static 'profiles/css/profile.css' %}">
{% endblock %}

{% block page_header %}
    <div class="container header-container">
        <div class="row">
            <div class="col"></div>
        </div>
    </div>
{% endblock %}

{% block content %}
    <div class="overlay"></div>
    <div class="container">
        <div class="row">
            <div class="col">
                <hr>
                <h2 class="logo-font mb-4">My Profile</h2>
                <hr>
            </div>
        </div>
        <div class="row">
            <div class="col-12 col-lg-6">
                <p class="text-muted">Default Delivery Information</p>
                <form class="mt-3" action="{% url 'profile' %}" method="POST" id="profile-update-form">
                    {% csrf_token %}
                    {{ form|crispy }}
                    <button class="btn btn-black rounded-0 text-uppercase float-right">Update Information</button>
                </form>
            </div>
            <div class="col-12 col-lg-6">
                <p class="text-muted">Order History</p>
                <div class="order-history table-responsive">
                    <table class="table table-sm table-borderless">
                        <thead>
                            <tr>
                                <th>Order Number</th>
                                <th>Date</th>
                                <th>Items</th>
                                <th>Order Total</th>
                            </tr>
                        </thead>
                        <tbody>
                            {% for order in orders %}
                                <tr>
                                    <td>
                                        <a href="{% url 'order_history' order.order_number %}"
                                        title="{{ order.order_number }}">
                                            {{ order.order_number|truncatechars:6 }}
                                        </a>
                                    </td>
                                    <td>{{ order.date }}</td>
                                    <td>
                                        <ul class="list-unstyled">
                                            {% for item in order.lineitems.all %}
                                                <li class="small">
                                                    {% if item.product.has_sizes %}
                                                        Size {{ item.product.size|upper }}
                                                    {% endif %}{{ item.product.name }} x{{ item.quantity }}
                                                </li>
                                            {% endfor %}
                                        </ul>
                                    </td>
                                    <td>${{ order.grand_total }}</td>
                                </tr>
                            {% endfor %}
                        </tbody>
                    </table>
                </div>
            </div>
        </div>
{% endblock %}

{% block postloadjs %}
    {{ block.super }}
    <script type="text/javascript" src="{% static 'profiles/js/countryfield.js' %}"></script>
{% endblock %}