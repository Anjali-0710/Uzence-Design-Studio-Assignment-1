# DataTable Component

A reusable and flexible DataTable built with React + TypeScript.

## Features
- Display tabular data
- Column sorting (ascending/descending)
- Row selection (single/multiple)
- Loading state
- Empty state
- Accessible with ARIA attributes

## Props
```ts
interface DataTableProps<T> {
  data: T[];
  columns: Column<T>[];
  loading?: boolean;
  selectable?: boolean;
  onRowSelect?: (selectedRows: T[]) => void;
}

interface Column<T> {
  key: string;
  title: string;
  dataIndex: keyof T;
  sortable?: boolean;
}
