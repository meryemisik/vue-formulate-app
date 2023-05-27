<template>
  <div class="form" >
    <FormulateForm
    :schema="items" >
       
   </FormulateForm>
  </div>
</template>
<script>
export default {
  data() {
    return {
      items: [
        {
          type: "group",
          children: [
            {
              type: "text",
              name: "Name",
              label: "Name",
            },
            {
              type: "text",
              name: "Surname",
              label: "Surname",
            },
            {
              type: "text",
              name: "Address",
              label: "Address",
            },
            {
              type: "radio",
              options: [
                {
                  value: "first",
                  id: "first",
                  label: "First",
                },
                {
                  value: "second",
                  id: "second",
                  label: "Second",
                },
              ],
            },
            {
              type: "textarea",
              name: "İnfo",
              label: "İnfo",
            },
            {
              type: "button",
              name: "Send",
              label: "Send",
            }
          ],
        },
      ],
    };
  },
};
</script>
<style>
.form {
 max-width: 70%;
  margin: auto;
  
}
</style>
