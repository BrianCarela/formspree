# Emails: Using a Contact Form
***

# How To

1. Go to the [Formspree Website](https://formspree.io/) and sign up for an account. Make sure you check your email and verify it!

2. Create a new form, call it anything. You should see a Form Endpoint, copy the code after the `/f/`.

3. Under "Code Examples", select the "React" tab. You will be using it to guide how you label and name your inputs! 

4. In your react app, run command `npm install @formspree/react`

5. Use the following import:

```jsx
import { useForm, ValidationError } from '@formspree/react';
```

6. Set up the `useForm` hook:

```jsx
const [state, handleSubmit] = useForm("<YOUR_EMAIL_CODE_HERE>")
```

Make sure to replace `<YOUR_EMAIL_CODE_HERE>` with the Form Endpoint code you copied earlier

7. Test it! It should send you an email with someone's submitted email and a message. Now integrate this contact form wherever you need it!