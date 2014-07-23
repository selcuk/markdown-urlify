# Markdown-URLify #

This Python-Markdown extension modifies the HTML output of Python-Markdown
such that URLs in the text becomes clickable links.

## Usage ##

Just instantiate the URLifyExtension class and pass it to the markdown method,
such as:

    import markdown
    import urlify

    def markdown_with_urlify(text):
        urlify_ext = urlify.URLifyExtension()
        extensions = [urlify_ext]
        return markdown.markdown(text, extensions)

For more information, see
[Python-Markdown Extension API documentation](https://pythonhosted.org/Markdown/extensions/api.html)
