# -showing-the-Step-Definition-for-verifying-for-a-specific-name-or-text-NOT-to-be-present
@then('I should not see "{text}" on the page')
def step_impl(context, text):
    assert text not in context.browser.page_source
