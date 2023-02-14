Time to connect the dots!

## Setup

1. Fork and clone [this repository](https://github.com/JoinCODED/TASK-Django-M6-Model-Relations).
2. Create a `virtual environment` and activate it.
3. Install the dependencies using `pip install -r requirements.txt`.

## Steps

1. Add a `many-to-many` relationship between `Course` and `Tag` (make sure to add an appropriate `related_name`).
   - Run `pytest -k many_to_many` to verify you have done this step correctly.
2. Add a `many-to-one` relationship between `Lecture` and `Course`, where `Lecture` is the _many_ in the relationship (make sure to add an appropriate `related_name`).
   - Run `pytest -k many_to_one` to verify you have done this step correctly.
3. Add a `one-to-one` relationship between `Lecture` and `Slide` (make sure to keep only one `primary key`).
4. Add a `one-to-one` relationship between `Lecture` and `Assignment` (make sure to keep only one `primary key`).
   - Run `pytest -k one_to_one` to verify you have done the two previous steps correctly.
5. Make migrations, migrate, and test out your code on the admin panel.
6. Run `pytest`, pass all steps, and push your code.

## Bonus

Use [model inheritance](https://docs.djangoproject.com/en/4.0/topics/db/models/#model-inheritance-1) to DRY up your code (i.e., cut out the code duplication in `Assignment` and `Slide`).
