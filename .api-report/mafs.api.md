## API Report File for "mafs"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import * as React_2 from 'react';
import * as vec from 'vec-la';
import { VFC } from 'react';

// @public (undocumented)
export type AxisOptions = {
    axis: boolean;
    lines: number | false;
    subdivisions: number | false;
    labels: false | LabelMaker;
};

// @public (undocumented)
export type CardinalDirection = "n" | "ne" | "e" | "se" | "s" | "sw" | "w" | "nw";

// @public (undocumented)
export const CartesianCoordinates: React_2.NamedExoticComponent<CartesianCoordinatesProps>;

// @public (undocumented)
export interface CartesianCoordinatesProps {
    // (undocumented)
    subdivisions?: number | false;
    // (undocumented)
    xAxis?: Partial<AxisOptions>;
    // (undocumented)
    yAxis?: Partial<AxisOptions>;
}

// @public (undocumented)
export const Circle: React_2.VFC<CircleProps>;

// @public (undocumented)
export interface CircleProps extends Filled {
    // (undocumented)
    center: Vector2;
    // (undocumented)
    radius: number;
    // (undocumented)
    svgEllipseProps?: React_2.SVGProps<SVGEllipseElement>;
}

// @public (undocumented)
export type ConstraintFunction = (position: Vector2) => Vector2;

// @public (undocumented)
export type _ConstraintFunction1 = (position: Vector2) => Vector2;

// @public (undocumented)
export const Ellipse: React_2.VFC<EllipseProps>;

// @public (undocumented)
export interface EllipseProps extends Filled {
    // (undocumented)
    angle?: number;
    // (undocumented)
    center: Vector2;
    // (undocumented)
    radius: Vector2;
    // (undocumented)
    svgEllipseProps?: React_2.SVGProps<SVGEllipseElement>;
}

// @public (undocumented)
export interface Filled {
    // (undocumented)
    color?: string;
    // (undocumented)
    fillOpacity?: number;
    // (undocumented)
    strokeOpacity?: number;
    // (undocumented)
    strokeStyle?: "solid" | "dashed";
    // (undocumented)
    weight?: number;
}

// @public (undocumented)
export const FunctionGraph: {
    OfX: VFC<OfXProps>;
    Parametric: VFC<ParametricProps>;
};

// @public (undocumented)
export type Interval = [min: number, max: number];

// @public (undocumented)
export type LabelMaker = (value: number) => number | string;

// @public (undocumented)
export function labelPi(x: number): string;

// @public (undocumented)
export const Line: {
    PointAngle: VFC<PointAngleProps>;
    PointSlope: VFC<PointSlopeProps>;
    ThroughPoints: VFC<ThroughPointsProps>;
    Segment: VFC<SegmentProps>;
};

// @public (undocumented)
export const Mafs: React_2.FC<MafsViewProps>;

// @public (undocumented)
export interface MafsViewProps {
    // (undocumented)
    height?: number;
    // (undocumented)
    pan?: boolean;
    ssr?: boolean;
    // (undocumented)
    width?: number | string;
    // (undocumented)
    xAxisExtent?: Interval;
    // (undocumented)
    yAxisExtent?: Interval;
}

// @public (undocumented)
export const MovablePoint: React_2.VFC<MovablePointProps>;

// @public (undocumented)
export interface MovablePointProps {
    // (undocumented)
    color?: string;
    constrain?: _ConstraintFunction1;
    onMove: (point: Vector2) => void;
    point: Vector2;
    transform?: vec.Matrix;
}

// @public (undocumented)
export interface OfXProps extends Stroked {
    // (undocumented)
    quality?: "low" | "medium" | "high";
    // (undocumented)
    svgPathProps?: React_2.SVGProps<SVGPathElement>;
    // (undocumented)
    y: (x: number) => number;
}

// @public (undocumented)
export interface ParametricProps extends Stroked {
    // (undocumented)
    color?: string;
    minimumSamplingDepth?: number;
    // @deprecated (undocumented)
    samples?: never;
    // (undocumented)
    style?: "solid" | "dashed";
    // (undocumented)
    svgPathProps?: React_2.SVGProps<SVGPathElement>;
    // (undocumented)
    t: [number, number];
    // (undocumented)
    xy: (t: number) => Vector2;
}

// @public (undocumented)
export const Point: React_2.VFC<PointProps>;

// @public (undocumented)
export interface PointAngleProps extends Stroked {
    // (undocumented)
    angle: number;
    // (undocumented)
    point: Vector2;
}

// @public (undocumented)
export interface PointProps {
    // (undocumented)
    color?: string;
    // (undocumented)
    opacity?: number;
    // (undocumented)
    svgCircleProps?: React_2.SVGProps<SVGCircleElement>;
    // (undocumented)
    x: number;
    // (undocumented)
    y: number;
}

// @public (undocumented)
export interface PointSlopeProps extends Stroked {
    // (undocumented)
    point: Vector2;
    // (undocumented)
    slope: number;
}

// @public (undocumented)
export const Polygon: React_2.VFC<PolygonProps>;

// @public (undocumented)
export interface PolygonProps extends Filled {
    // (undocumented)
    points: Vector2[];
    // (undocumented)
    svgPolygonProps?: React_2.SVGProps<SVGPolygonElement>;
}

// @public (undocumented)
export interface SegmentProps extends Stroked {
    // (undocumented)
    point1: Vector2;
    // (undocumented)
    point2: Vector2;
}

// @public (undocumented)
export interface Stopwatch {
    setTime: (time: number) => void;
    start: () => void;
    stop: () => void;
    time: number;
}

// @public (undocumented)
export interface StopwatchArguments {
    endTime?: number;
    startTime?: number;
}

// @public (undocumented)
export interface Stroked {
    // (undocumented)
    color?: string;
    // (undocumented)
    opacity?: number;
    // (undocumented)
    style?: "solid" | "dashed";
    // (undocumented)
    weight?: number;
}

// @public (undocumented)
const Text_2: React_2.FC<TextProps>;
export { Text_2 as Text }

// @public (undocumented)
export interface TextProps {
    // (undocumented)
    attach?: CardinalDirection;
    // (undocumented)
    attachDistance?: number;
    // (undocumented)
    color?: string;
    // (undocumented)
    size?: number;
    // (undocumented)
    svgTextProps?: React_2.SVGAttributes<SVGTextElement>;
    // (undocumented)
    x: number;
    // (undocumented)
    y: number;
}

// @public (undocumented)
export const Theme: {
    foreground: string;
    background: string;
    red: string;
    orange: string;
    green: string;
    blue: string;
    indigo: string;
    violet: string;
    pink: string;
    yellow: string;
};

// @public (undocumented)
export interface ThroughPointsProps extends Stroked {
    // (undocumented)
    point1: Vector2;
    // (undocumented)
    point2: Vector2;
}

// @public (undocumented)
export interface UseMovablePoint {
    // (undocumented)
    element: React_2.ReactElement;
    // (undocumented)
    point: Vector2;
    // (undocumented)
    setPoint: (point: Vector2) => void;
    // (undocumented)
    x: number;
    // (undocumented)
    y: number;
}

// @public (undocumented)
export function useMovablePoint(initialPoint: Vector2, { constrain, color, transform }?: UseMovablePointArguments): UseMovablePoint;

// @public (undocumented)
export interface UseMovablePointArguments {
    // (undocumented)
    color?: string;
    constrain?: "horizontal" | "vertical" | ConstraintFunction;
    transform?: vec.Matrix;
}

// @public (undocumented)
export function useStopwatch(options?: StopwatchArguments): Stopwatch;

// @public (undocumented)
export const Vector: React_2.VFC<VectorProps>;

// @public (undocumented)
export type Vector2 = [x: number, y: number];

// @public (undocumented)
export const VectorField: React_2.VFC<VectorFieldProps>;

// @public (undocumented)
export interface VectorFieldProps {
    // (undocumented)
    color?: string;
    // (undocumented)
    opacityStep?: number;
    // (undocumented)
    step: number;
    // (undocumented)
    xy: (x: number, y: number) => [number, number];
    // (undocumented)
    xyOpacity?: (x: number, y: number) => number;
}

// @public (undocumented)
export interface VectorProps extends Stroked {
    // (undocumented)
    svgLineProps?: React_2.SVGProps<SVGLineElement>;
    // (undocumented)
    tail?: Vector2;
    // (undocumented)
    tip: Vector2;
}

// (No @packageDocumentation comment for this package)

```
