## Tokens Overview

```mermaid
graph LR;
    cbar[CBAR Design];
    cbar --> cbar.sys[System];
    cbar --> cbar.ref[Reference];

    cbar.ref --> cbar.ref.palette[Palette];

    cbar.ref.palette --> primary(Primary);
    primary ----> cbar.ref.palette.primary0[Primary 0];
    primary ----> cbar.ref.palette.primary10[Primary 10];
    primary ----> cbar.ref.palette.primary20[Primary 20];
    primary ----> cbar.ref.palette.primary30[Primary 30];
    primary ----> cbar.ref.palette.primary40[Primary 40];
    primary ----> cbar.ref.palette.primary50[Primary 50];
    primary ----> cbar.ref.palette.primary60[Primary 60];
    primary ----> cbar.ref.palette.primary70[Primary 70];
    primary ----> cbar.ref.palette.primary80[Primary 80];
    primary ----> cbar.ref.palette.primary90[Primary 90];
    primary ----> cbar.ref.palette.primary95[Primary 95];
    primary ----> cbar.ref.palette.primary99[Primary 99];
    primary ----> cbar.ref.palette.primary100[Primary 100];

    cbar.ref.palette --> secondary(Secondary);
    secondary ----> cbar.ref.palette.secondary0[Secondary 0];
    secondary ----> cbar.ref.palette.secondary10[Secondary 10];
    secondary ----> cbar.ref.palette.secondary20[Secondary 20];
    secondary ----> cbar.ref.palette.secondary30[Secondary 30];
    secondary ----> cbar.ref.palette.secondary40[Secondary 40];
    secondary ----> cbar.ref.palette.secondary50[Secondary 50];
    secondary ----> cbar.ref.palette.secondary60[Secondary 60];
    secondary ----> cbar.ref.palette.secondary70[Secondary 70];
    secondary ----> cbar.ref.palette.secondary80[Secondary 80];
    secondary ----> cbar.ref.palette.secondary90[Secondary 90];
    secondary ----> cbar.ref.palette.secondary95[Secondary 95];
    secondary ----> cbar.ref.palette.secondary99[Secondary 99];
    secondary ----> cbar.ref.palette.secondary100[Secondary 100];

    cbar.ref.palette --> tertiary(Tertiary);
    tertiary ----> cbar.ref.palette.tertiary0[Tertiary 0];
    tertiary ----> cbar.ref.palette.tertiary10[Tertiary 10];
    tertiary ----> cbar.ref.palette.tertiary20[Tertiary 20];
    tertiary ----> cbar.ref.palette.tertiary30[Tertiary 30];
    tertiary ----> cbar.ref.palette.tertiary40[Tertiary 40];
    tertiary ----> cbar.ref.palette.tertiary50[Tertiary 50];
    tertiary ----> cbar.ref.palette.tertiary60[Tertiary 60];
    tertiary ----> cbar.ref.palette.tertiary70[Tertiary 70];
    tertiary ----> cbar.ref.palette.tertiary80[Tertiary 80];
    tertiary ----> cbar.ref.palette.tertiary90[Tertiary 90];
    tertiary ----> cbar.ref.palette.tertiary95[Tertiary 95];
    tertiary ----> cbar.ref.palette.tertiary99[Tertiary 99];
    tertiary ----> cbar.ref.palette.tertiary100[Tertiary 100];

    cbar.ref.palette --> neutral(Neutral);
    neutral ----> cbar.ref.palette.neutral0[Neutral 0];
    neutral ----> cbar.ref.palette.neutral10[Neutral 10];
    neutral ----> cbar.ref.palette.neutral20[Neutral 20];
    neutral ----> cbar.ref.palette.neutral30[Neutral 30];
    neutral ----> cbar.ref.palette.neutral40[Neutral 40];
    neutral ----> cbar.ref.palette.neutral50[Neutral 50];
    neutral ----> cbar.ref.palette.neutral60[Neutral 60];
    neutral ----> cbar.ref.palette.neutral70[Neutral 70];
    neutral ----> cbar.ref.palette.neutral80[Neutral 80];
    neutral ----> cbar.ref.palette.neutral90[Neutral 90];
    neutral ----> cbar.ref.palette.neutral95[Neutral 95];
    neutral ----> cbar.ref.palette.neutral99[Neutral 99];
    neutral ----> cbar.ref.palette.neutral100[Neutral 100];

    cbar.ref.palette --> neutralVariant(Neutral Variant);
    neutralVariant ----> cbar.ref.palette.neutral-variant0[Neutral Variant 0];
    neutralVariant ----> cbar.ref.palette.neutral-variant10[Neutral Variant 10];
    neutralVariant ----> cbar.ref.palette.neutral-variant20[Neutral Variant 20];
    neutralVariant ----> cbar.ref.palette.neutral-variant30[Neutral Variant 30];
    neutralVariant ----> cbar.ref.palette.neutral-variant40[Neutral Variant 40];
    neutralVariant ----> cbar.ref.palette.neutral-variant50[Neutral Variant 50];
    neutralVariant ----> cbar.ref.palette.neutral-variant60[Neutral Variant 60];
    neutralVariant ----> cbar.ref.palette.neutral-variant70[Neutral Variant 70];
    neutralVariant ----> cbar.ref.palette.neutral-variant80[Neutral Variant 80];
    neutralVariant ----> cbar.ref.palette.neutral-variant90[Neutral Variant 90];
    neutralVariant ----> cbar.ref.palette.neutral-variant95[Neutral Variant 95];
    neutralVariant ----> cbar.ref.palette.neutral-variant99[Neutral Variant 99];
    neutralVariant ----> cbar.ref.palette.neutral-variant100[Neutral Variant 100];

    cbar.ref.palette --> error(Error);
    error ----> cbar.ref.palette.error0[Error 0];
    error ----> cbar.ref.palette.error10[Error 10];
    error ----> cbar.ref.palette.error20[Error 20];
    error ----> cbar.ref.palette.error30[Error 30];
    error ----> cbar.ref.palette.error40[Error 40];
    error ----> cbar.ref.palette.error50[Error 50];
    error ----> cbar.ref.palette.error60[Error 60];
    error ----> cbar.ref.palette.error70[Error 70];
    error ----> cbar.ref.palette.error80[Error 80];
    error ----> cbar.ref.palette.error90[Error 90];
    error ----> cbar.ref.palette.error95[Error 95];
    error ----> cbar.ref.palette.error100[Error 100];

    cbar.sys --> cbar.sys.color[Color];

    cbar.sys.color ----> cbar.sys.color.primary[Primary];
    cbar.sys.color.primary --Light---> cbar.ref.palette.primary40;
    cbar.sys.color.primary --Dark---> cbar.ref.palette.primary80;
    cbar.sys.color ----> cbar.sys.color.onPrimary[On Primary];
    cbar.sys.color.onPrimary --Light---> cbar.ref.palette.primary100;
    cbar.sys.color.onPrimary --Dark---> cbar.ref.palette.primary20;
    cbar.sys.color ----> cbar.sys.color.primaryContainer[Primary Container];
    cbar.sys.color.primaryContainer --Light---> cbar.ref.palette.primary90;
    cbar.sys.color.primaryContainer --Dark---> cbar.ref.palette.primary30;
    cbar.sys.color ----> cbar.sys.color.onPrimaryContainer[On Primary Container];
    cbar.sys.color.onPrimaryContainer --Light---> cbar.ref.palette.primary10;
    cbar.sys.color.onPrimaryContainer --Dark---> cbar.ref.palette.primary90;

    cbar.sys.color ----> cbar.sys.color.secondary[Secondary];
    cbar.sys.color.secondary --Light---> cbar.ref.palette.secondary40;
    cbar.sys.color.secondary --Dark---> cbar.ref.palette.secondary80;
    cbar.sys.color ----> cbar.sys.color.onSecondary[On Secondary];
    cbar.sys.color.onSecondary --Light---> cbar.ref.palette.secondary100;
    cbar.sys.color.onSecondary --Dark---> cbar.ref.palette.secondary20;
    cbar.sys.color ----> cbar.sys.color.secondaryContainer[Secondary Container];
    cbar.sys.color.secondaryContainer --Light---> cbar.ref.palette.secondary90;
    cbar.sys.color.secondaryContainer --Dark---> cbar.ref.palette.secondary30;
    cbar.sys.color ----> cbar.sys.color.onSecondaryContainer[On Secondary Container];
    cbar.sys.color.onSecondaryContainer --Light---> cbar.ref.palette.secondary10;
    cbar.sys.color.onSecondaryContainer --Dark---> cbar.ref.palette.secondary90;

    cbar.sys.color ----> cbar.sys.color.tertiary[Tertiary];
    cbar.sys.color.tertiary --Light---> cbar.ref.palette.tertiary40;
    cbar.sys.color.tertiary --Dark---> cbar.ref.palette.tertiary80;
    cbar.sys.color ----> cbar.sys.color.onTertiary[On Tertiary];
    cbar.sys.color.onTertiary --Light---> cbar.ref.palette.tertiary100;
    cbar.sys.color.onTertiary --Dark---> cbar.ref.palette.tertiary20;
    cbar.sys.color ----> cbar.sys.color.tertiaryContainer[Tertiary Container];
    cbar.sys.color.tertiaryContainer --Light---> cbar.ref.palette.tertiary90;
    cbar.sys.color.tertiaryContainer --Dark---> cbar.ref.palette.tertiary30;
    cbar.sys.color ----> cbar.sys.color.onTertiaryContainer[On Tertiary Container];
    cbar.sys.color.onTertiaryContainer --Light---> cbar.ref.palette.tertiary10;
    cbar.sys.color.onTertiaryContainer --Dark---> cbar.ref.palette.tertiary90;

    cbar.sys.color ----> cbar.sys.color.error[Error];
    cbar.sys.color.error --Light---> cbar.ref.palette.error40;
    cbar.sys.color.error --Dark---> cbar.ref.palette.error80;
    cbar.sys.color ----> cbar.sys.color.onError[On Error];
    cbar.sys.color.onError --Light---> cbar.ref.palette.error100;
    cbar.sys.color.onError --Dark---> cbar.ref.palette.error20;
    cbar.sys.color ----> cbar.sys.color.errorContainer[Error Container];
    cbar.sys.color.errorContainer --Light---> cbar.ref.palette.error90;
    cbar.sys.color.errorContainer --Dark---> cbar.ref.palette.error30;
    cbar.sys.color ----> cbar.sys.color.onErrorContainer[On Error Container];
    cbar.sys.color.onErrorContainer --Light---> cbar.ref.palette.error10;
    cbar.sys.color.onErrorContainer --Dark---> cbar.ref.palette.error90;

    cbar.sys.color ----> cbar.sys.color.background[Background];
    cbar.sys.color.background --Light---> cbar.ref.palette.neutral99;
    cbar.sys.color.background --Dark---> cbar.ref.palette.neutral10;
    cbar.sys.color ----> cbar.sys.color.onBackground[On Background];
    cbar.sys.color.onBackground --Light---> cbar.ref.palette.neutral10;
    cbar.sys.color.onBackground --Dark---> cbar.ref.palette.neutral90;

    cbar.sys.color ----> cbar.sys.color.surface[Surface];
    cbar.sys.color.surface --Light---> cbar.ref.palette.neutral99;
    cbar.sys.color.surface --Dark---> cbar.ref.palette.neutral10;
    cbar.sys.color ----> cbar.sys.color.onSurface[On Surface];
    cbar.sys.color.onSurface --Light---> cbar.ref.palette.neutral10;
    cbar.sys.color.onSurface --Dark---> cbar.ref.palette.neutral90;

    cbar.sys.color ----> cbar.sys.color.surfaceVariant[Surface Variant];
    cbar.sys.color.surfaceVariant --Light---> cbar.ref.palette.neutral-variant90;
    cbar.sys.color.surfaceVariant --Dark---> cbar.ref.palette.neutral-variant30;
    cbar.sys.color ----> cbar.sys.color.onSurfaceVariant[On Surface Variant];
    cbar.sys.color.onSurfaceVariant --Light---> cbar.ref.palette.neutral-variant30;
    cbar.sys.color.onSurfaceVariant --Dark---> cbar.ref.palette.neutral-variant80;

    cbar.sys.color ----> cbar.sys.color.inverseSurface[Inverse Surface];
    cbar.sys.color.inverseSurface --Light---> cbar.ref.palette.neutral20;
    cbar.sys.color.inverseSurface --Dark---> cbar.ref.palette.neutral90;
    cbar.sys.color ----> cbar.sys.color.inverseOnSurface[Inverse On Surface];
    cbar.sys.color.inverseOnSurface --Light---> cbar.ref.palette.neutral95;
    cbar.sys.color.inverseOnSurface --Dark---> cbar.ref.palette.neutral20;
    
    cbar.sys.color ----> cbar.sys.color.surfaceTint[Surface Tint] ---> cbar.sys.color.primary;
    
    cbar.sys.color ----> cbar.sys.color.outline[Outline];
    cbar.sys.color.outline --Light---> cbar.ref.palette.neutral-variant50;
    cbar.sys.color.outline --Dark---> cbar.ref.palette.neutral60;

    cbar.sys.color ----> cbar.sys.color.shadow[Shadow];
    cbar.sys.color.shadow --Light---> cbar.ref.palette.neutral0;
    cbar.sys.color.shadow --Dark---> cbar.ref.palette.neutral0;

    cbar.sys.color ----> cbar.sys.color.inversePrimary[Inverse Primary];
    cbar.sys.color.inversePrimary --Light---> cbar.ref.palette.primary80;
    cbar.sys.color.inversePrimary --Dark---> cbar.ref.palette.primary40;

```
