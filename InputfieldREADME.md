# InputField Component

A flexible and reusable Input component built with React + TypeScript.

## Features
- Label, placeholder, helper text, error message
- Validation states: disabled, invalid, loading
- Variants: filled, outlined, ghost
- Sizes: small, medium, large
- Optional: clear button, password toggle
- Light/Dark theme support
- Accessible with ARIA labels

## Props
```ts
interface InputFieldProps {
  value?: string;
  onChange?: (e: React.ChangeEvent<HTMLInputElement>) => void;
  label?: string;
  placeholder?: string;
  helperText?: string;
  errorMessage?: string;
  disabled?: boolean;
  invalid?: boolean;
  variant?: 'filled' | 'outlined' | 'ghost';
  size?: 'sm' | 'md' | 'lg';
}
