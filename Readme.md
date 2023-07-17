# Tables in HTML
# HTML Tables

This README provides an overview of HTML tables and how to use them in your web pages. Tables are a fundamental part of HTML and allow you to organize and present data in a structured manner. By using HTML table elements, you can create rows and columns of data that are easy to understand and navigate.

## Table of Contents
1. [Basic Table Structure](#basic-table-structure)
2. [Table Header](#table-header)
3. [Table Body](#table-body)
4. [Table Footer](#table-footer)
5. [Table Cell Types](#table-cell-types)
6. [Spanning Rows and Columns](#spanning-rows-and-columns)
7. [Styling Tables](#styling-tables)

## 1. Basic Table Structure

To create an HTML table, you need to use the `<table>` element. Inside the table, you define the table rows using the `<tr>` element, and within each row, you define table cells using the `<td>` element. Here's a basic example:

```html
<table>
  <tr>
    <td>Row 1, Cell 1</td>
    <td>Row 1, Cell 2</td>
  </tr>
  <tr>
    <td>Row 2, Cell 1</td>
    <td>Row 2, Cell 2</td>
  </tr>
</table>

##2.Table Header
To define a table header, you should use the <thead> element. Inside the <thead>, you define the header row using the <tr> element, and within each header cell, you use the <th> element instead of <td>. Here's an example:

<table>
  <thead>
    <tr>
      <th>Header 1</th>
      <th>Header 2</th>
    </tr>
  </thead>
  <tbody>
    <!-- table body rows -->
  </tbody>
</table>

##3.Table Body
The actual data of the table is placed within the <tbody> element. It contains the rows and cells that make up the body of the table. Here's an example:

    <table>
  <thead>
    <!-- table header row(s) -->
  </thead>
  <tbody>
    <tr>
      <td>Data 1</td>
      <td>Data 2</td>
    </tr>
    <tr>
      <td>Data 3</td>
      <td>Data 4</td>
    </tr>
  </tbody>
</table>

##4.Table Footer
If you have a footer section for your table, you can use the <tfoot> element. Similar to the <thead>, you define the footer row using the <tr> element, and within each footer cell, you use the <td> or <th> element. Here's an example:
    <table>
  <thead>
    <!-- table header row(s) -->
  </thead>
  <tbody>
    <!-- table body rows -->
  </tbody>
  <tfoot>
    <tr>
      <td>Footer 1</td>
      <td>Footer 2</td>
    </tr>
  </tfoot>
</table>

You can have multiple rows in the <tfoot> if needed.

##5.Table Cell Types
Table cells can contain various types of content such as text, images, links, or even nested tables. You can include any valid HTML content within the <td> or <th> elements.

##6.Spanning Rows and Columns
You can span rows or columns by using the rowspan and colspan attributes respectively. These attributes allow a cell to occupy multiple rows or columns. Here's an example:


<table>
  <tr>
    <td rowspan="2">Spanning Cell</td>
    <td>Cell 1</td>
    <td>Cell 2</td>
  </tr>
  <tr>
    <td colspan="2">Spanned Cells</td>
  </tr>
</table>
The above code creates a table with a cell that spans two rows and another cell that spans two columns.

##7.Styling Tables
You can apply CSS styles to tables and their elements to customize their appearance. You can use inline styles or define styles in an external CSS file.

For example, you can add a class to the table element and define styles for that class in your CSS:

html
Copy code
<style>
  .custom-table {
    border-collapse: collapse;
    width: 100%;
  }
  .custom-table th, .custom-table td {
    border: 1px solid black;
    padding: 8px;
    text-align: left;
  }
</style>

<table class="custom-table">
  <!-- table content -->
</table>

In this example, the table has a custom class name "custom-table," and the CSS styles define a border, padding, and text alignment for the table cells.

That's it! You now have a basic understanding of HTML tables and how to use them in your web pages. Happy coding!
