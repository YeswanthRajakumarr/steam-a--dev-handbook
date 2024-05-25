---
sidebar_position: 1
---

# Purpose of this Hand

This handbook is a guide for developers within an organization, outlining coding standards, best practices, tools, processes, and conventions. Its purpose is to ensure consistency, efficiency, and collaboration across development teams by providing a centralized resource for onboarding, reference, and knowledge sharing. Additionally, it helps maintain code quality, streamline workflows, and foster a common understanding of development practices among team members.

## Ground Rules

### Do's

- **Use React Router** for client-side routing to manage navigation within the application.
- **Implement lazy loading** for components and routes to improve initial load times and reduce bandwidth usage.
- **Utilize React Context or Redux** for state management, especially for global application state or complex data flows.
- **Write clear and concise comments** to document complex logic or functionality for easier understanding by other developers.
- **Use PropTypes or TypeScript** for type checking and validation of props passed to components.
- **Implement accessibility features** such as ARIA attributes and keyboard navigation for improved usability for users with disabilities.
- **Employ React Hooks** for managing state and side effects in functional components, promoting code reuse and readability.
- **Utilize PureComponent or React.memo** for optimizing performance by preventing unnecessary re-renders of components.
- **Implement server-side rendering (SSR) or static site generation (SSG)** for improved SEO and initial load performance.
- **Write unit tests** using Jest and React Testing Library to ensure the reliability and correctness of components and functions.
- **Regularly update dependencies** to leverage new features, bug fixes, and security patches, while ensuring compatibility with the latest versions of React and related libraries.
- **Maintain consistency** by keeping folder names, file names, and exported component/layout names the same prefix with different suffixes.
- **Ensure responsive layouts** for optimal user experience.
- **Follow a modular structure** for easier code organization and maintenance.
- **Utilize Ant Design components** for consistent UI elements and layouts.
- **Implement code linting and formatting tools** for code consistency.
- **Optimize images and assets** for faster page loading times.
- **Implement error handling and validation** for user input forms.
- **Leverage Ant Design's grid system** for responsive layouts.
- **Follow Ant Design's design guidelines** for a cohesive user experience.
- **Utilize Ant Design's form components** for efficient form management.
- **Use Ant Design's icon library** for consistent and visually appealing icons.
- **Utilize React's component lifecycle methods** for efficient state management.

### Don'ts

- **Avoid using index as keys** for lists, as it can lead to performance issues and unexpected behavior when items are added, removed, or reordered.
- **Refrain from manipulating the DOM directly** outside of React's lifecycle methods or hooks, as it can lead to inconsistencies and bugs.
- **Avoid using setState inside useEffect** without proper dependency management, as it can cause infinite loops or unnecessary re-renders.
- **Steer clear of using browser-specific APIs directly in components**, as it can lead to cross-browser compatibility issues.
- **Avoid excessive nesting of components**, as it can make the code harder to understand and maintain.
- **Refrain from using setState in the constructor**, as it can lead to unexpected behavior due to the asynchronous nature of setState.
- **Avoid using inline event handlers in JSX**, as it can make the code less readable and harder to maintain.
- **Minimize the use of forceUpdate**, as it bypasses React's reconciliation process and can lead to unpredictable behavior.
- **Avoid relying solely on client-side validation** for sensitive data or security-critical operations, as it can be bypassed by malicious users.
- **Refrain from using componentWillReceiveProps, componentWillMount, and other deprecated lifecycle methods**, as they may be removed in future versions of React.
- **Avoid relying on internal implementation details of third-party libraries**, as they may change without notice and break your application.
- **Avoid writing custom CSS** to maintain consistency and prevent styling conflicts.
- **Utilize Row tags with at least 2 Col tags inside** to maintain layout structure; otherwise, refrain from using Row.
- **Avoid using the state from the previous page** to prevent unexpected behavior.
- **Replace `<br />` tags or margins** with a parent Row wrapper with gutter spacing and Col wrappers for each Row section.
- **Avoid using inline styles** to maintain separation of concerns.
- **Refrain from using deprecated or nonstandard HTML tags and attributes.**
- **Minimize the use of nested components** to prevent performance issues.
- **Avoid hardcoding values** where constants or variables could be used instead.
- **Steer clear of excessive dependencies** to keep the project lightweight and maintainable.
- **Refrain from using outdated or vulnerable libraries** to ensure security.
