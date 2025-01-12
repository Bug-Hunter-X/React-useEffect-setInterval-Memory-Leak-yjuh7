# React useEffect setInterval Memory Leak
This example demonstrates a common error in React: a memory leak caused by improper use of the setInterval function inside the useEffect hook.

The bug is in the `MyComponent` component where the setInterval function is used without proper cleanup.  This leads to the interval continuing even after the component unmounts, resulting in a memory leak.

The solution shows how to fix this by adding a cleanup function to clear the interval when the component unmounts.