# Testing Red Hat Operators on FIPS-enabled clusters

[Spreadsheet](https://docs.google.com/spreadsheets/d/1laoPFNv78K2nm4BKZxPRAJK24DNqMq8smaoFnHvbUb4/edit#gid=0)

# Data to be set from an assessment

A pass/fail should be set in facts to communicate to the caller the result.
As of now, this is a simple string of "pass" or "fail":

```
- name: Create result
  ansible.builtin.set_fact:
    assessment_result: "{{ test_result }}"
```
