# Decision Records Management

This guide provides step-by-step instructions for developers to create decision records.

## Creating a New Decision Record

### Adopted Solution

!!! success "Solution Adopted"
    1. In the `adopted` directory, create a new markdown file for the decision record.
    2. Name the file using the format `<short-description>.md`, replacing `<short-description>` with a brief description of the decision. For example, `standardize-html-img-tag.md`
    3. Use the Decision Record Template provided below, and fill in the relevant information for your decision record.
    4. Once you have created the new decision record file, make sure to include it in the [List of Decision Records](index.md#list-of-decision-records) section in the `docs/DR/index.md` page.
    ``` markdown

    ---
    status: ✅ Adopted
    ---

    #### Issue
    [#<issue_number>](https://github.com/hackforla/website/issues/<issue_number>) or None

    #### Problem Statement
    Explain the problem you're trying to solve in more detail.

    #### Potential Solution
    Describe the potential solution that was evaluated.

    #### Feasibility Determination
    Explain how the feasibility of the potential solution was determined, including any factors that influenced the decision (time, resources, etc.).

    #### Sources
    If applicable, include any relevant source links here.
    ```

### Not Implemented Solution

!!! failure "Solution Not Implemented"
    1. In the `not_implemented` directory, create a new markdown file for the decision record.
    2. Name the file using the format `<short-description>.md`, replacing `<short-description>` with a brief description of the decision.
    3. Use the Decision Record Template provided below, and fill in the relevant information for your decision record.
    4. Once you have created the new decision record file, make sure to include it in the [List of Decision Records](index.md#list-of-decision-records) section in the `docs/DR/index.md` page.
    ``` markdown

    ---
    status: ⛔ Not Implemented
    ---

    #### Issue
    [#<issue_number>](https://github.com/hackforla/website/issues/<issue_number>) or None

    #### Problem Statement
    Explain the problem you're trying to solve in more detail.

    #### Potential Solution
    Describe the potential solution that was evaluated.

    #### Feasibility Determination
    Explain how the feasibility of the potential solution was determined, including any factors that influenced the decision (time, resources, etc.).

    #### Sources
    If applicable, include any relevant source links here.
    ```
