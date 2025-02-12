## API Report File for "@fluentui/react-priority-overflow"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import type { ObserveOptions } from '@fluentui/priority-overflow';
import type { OnUpdateItemVisibility } from '@fluentui/priority-overflow';
import type { OnUpdateOverflow } from '@fluentui/priority-overflow';
import { OverflowGroupState } from '@fluentui/priority-overflow';
import type { OverflowItemEntry } from '@fluentui/priority-overflow';
import * as React_2 from 'react';

// @public (undocumented)
export const DATA_OVERFLOW_ITEM = "data-overflow-item";

// @public (undocumented)
export const DATA_OVERFLOW_MENU = "data-overflow-menu";

// @public (undocumented)
export const DATA_OVERFLOWING = "data-overflowing";

// @public (undocumented)
export const Overflow: React_2.ForwardRefExoticComponent<OverflowProps & React_2.RefAttributes<HTMLDivElement>>;

// @public (undocumented)
export interface OverflowProps extends React_2.HTMLAttributes<HTMLDivElement>, Pick<ObserveOptions, 'overflowAxis' | 'overflowDirection' | 'padding' | 'minimumVisible'> {
}

// @public (undocumented)
export const updateVisibilityAttribute: OnUpdateItemVisibility;

// @public (undocumented)
export function useIsOverflowGroupVisible(id: string): OverflowGroupState;

// @public (undocumented)
export function useIsOverflowItemVisible(id: string): boolean;

// @public (undocumented)
export const useOverflowContainer: <TElement extends HTMLElement>(update: OnUpdateOverflow, options: Omit<ObserveOptions, 'onUpdateOverflow'>) => UseOverflowContainerReturn<TElement>;

// @public (undocumented)
export interface UseOverflowContainerReturn<TElement extends HTMLElement> {
    containerRef: React_2.RefObject<TElement>;
    registerItem: OverflowContextValue['registerItem'];
    updateOverflow: OverflowContextValue['updateOverflow'];
}

// @public (undocumented)
export const useOverflowCount: () => number;

// @public
export function useOverflowItem<TElement extends HTMLElement>(id: string, priority?: number, groupId?: string): React_2.RefObject<TElement>;

// @public (undocumented)
export function useOverflowMenu<TElement extends HTMLElement>(id?: string): {
    ref: React_2.RefObject<TElement>;
    overflowCount: number;
    isOverflowing: boolean;
};

// (No @packageDocumentation comment for this package)

```
