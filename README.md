# Incorrect State Update in React Component

This repository demonstrates a common error in React components: using the deprecated `componentWillReceiveProps` lifecycle method and not handling undefined initial props. The original code uses `componentWillReceiveProps` to update the component's state when the `initialData` prop changes. However, this method is deprecated and can lead to unexpected behavior.

The solution uses `getDerivedStateFromProps` as a replacement to handle props change. It provides a way to handle undefined initial props and ensures the component updates correctly.  The solution also shows how to initialize the component's state in the constructor to a default value if `initialData` is initially undefined. 