# django-materialize-forms
Django tamplatetags for materialize css



Installation
------------
1. Install using pip:

    pip install django-materialize-forms

2. Add to INSTALLED_APPS:

    'materialize_forms',



Use in templates
----------------

    {% load materialize %}

    # Using a filter

    <form action="/url/to/submit/" method="post">
        {% csrf_token %}
        {{ form.field_1|as_material:"s12" }}
        {{ form.field_2|as_material:"s12" }}
        {{ form.field_3|as_material:"s12" }}
        <div class="form-actions">
            <button type="submit" class="btn btn-primary">Submit</button>
        </div>
    </form>
