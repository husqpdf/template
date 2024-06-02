<template>
  <pdf-document margin="15mm">
    <pdf-page>
      <h1>Welcome to HusqPDF</h1>
      <p>HusqPDF is an npm project tool that allows you to create PDF files using Vue.js. Follow the instructions below
        to get started.</p>

      <h2>1. Getting Started</h2>
      <p>To add PDF pages, create Vue files in the root folder <code>documents/[name]/index.vue</code>. Replace <code>[name]</code>
        with the desired name of your document.</p>

      <h2>2. Web Views</h2>
      <p>You can preview a page by visiting <code>/[name]#preview</code>. During development, you can add and modify
        page data by visiting <code>/[name]#develop</code>.</p>

      <h2>3. Add Schemas</h2>
      <p>Add JSON schema objects to the directory <code>schemas/[name]/schema.json</code>. These schemas define the data
        that the PDF document in <code>documents/[name]</code> should receive.</p>

      <h2>4. How to Generate the PDF</h2>
      <p>There is a POST endpoint at <code>/api/generate/[name]</code>. Send the data as a POST body to this endpoint
        and you will receive the generated PDF document.</p>
    </pdf-page>
  </pdf-document>
</template>

<style lang="css" scoped>
h1, h2 {
  font-weight: bold;
  margin-block: 1.25rem !important;
}

h1 {
  font-size: 3rem;
}

h2 {
  font-size: 1.75rem;
}

code {
  background: #f4f4f4;
  color: hsl(var(--primary));
  padding: 3px 6px !important;
  border-radius: 4px;
}
</style>