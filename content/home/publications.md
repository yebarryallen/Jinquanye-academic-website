widget: pages
headless: true  # This file represents a page section.

# ... Put Your Section Options Here (title etc.) ...

content:
  # Filter content to display
  filters:
    folders:
      - post
    tag: ''
    category: ''
    publication_type: ''
    author: ''
    exclude_featured: false
    exclude_future: false
    exclude_past: false
  # Choose how many pages you would like to display (0 = all pages)
  count: 10
  # Choose how many pages you would like to offset by
  offset: 0
  # Page order. Descending (desc) or ascending (asc) date.
  order: desc
design:
  # Toggle between the various page layout types. 
  view: compact
  columns: '2'
