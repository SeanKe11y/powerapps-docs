<properties
    pageTitle="Text-input control: reference | Microsoft PowerApps"
    description="Information, including properties and examples, about the text-input control"
    services=""
    suite="powerapps"
    documentationCenter="na"
    authors="aftowen"
    manager="erikre"
    editor=""
    tags=""/>

<tags
   ms.service="powerapps"
   ms.devlang="na"
   ms.topic="article"
   ms.tgt_pltfrm="na"
   ms.workload="na"
   ms.date="02/29/2016"
   ms.author="anneta"/>

# Text input control in PowerApps #
[AZURE.INCLUDE [control-summary-text-input](../../includes/control-summary-text-input.md)]

## Description ##
The user can specify data by typing into a text-input control. Depending on how you configure the app, that data might be added to a data source, used to calculate a temporary value, or incorporated in some other way.

## Key properties ##

**[Default](../properties/properties-core.md)** – The initial value of a control before it is changed by the user.

**[Text](../properties/properties-core.md)** – Text that appears on a control or that the user types into a control.

## Additional properties ##

**[Align](../properties/properties-text.md)** – The location of text in relation to the horizontal center of its control.

**[BorderColor](../properties/properties-color-border.md)** – The color of a control's border.

**[BorderStyle](../properties/properties-color-border.md)** – Whether a control's border is **Solid**, **Dashed**, **Dotted**, or **None**.

**[BorderThickness](../properties/properties-color-border.md)** – The thickness of a control's border.

**Clear** – Whether a text-input control shows an "X" that the user can tap or click to clear the contents of that control.

**[Color](../properties/properties-color-border.md)** – The color of text in a control.

**[Disabled](../properties/properties-core.md)** – Whether the user can interact with the control.

**[DisabledBorderColor](../properties/properties-color-border.md)** – The color of a control's border if the control's **Disabled** property is set to **true**.

**[DisabledColor](../properties/properties-color-border.md)** – The color of text in a control if its **Disabled** property is set to **true**.

**[DisabledFill](../properties/properties-color-border.md)** – The background color of a control if its **Disabled** property is set to **true**.

**[Fill](../properties/properties-color-border.md)** – The background color of a control.

**[Font](../properties/properties-text.md)** – The name of the family of fonts in which text appears.

**[FontWeight](../properties/properties-text.md)** – The weight of the text in a control: **Bold**, **Semibold**, **Normal**, or **Lighter**.

**[Height](../properties/properties-size-location.md)** – The distance between a control's top and bottom edges.

**HintText** – Light-grey text that appears in an input-text control if it's empty.

**[HoverBorderColor](../properties/properties-color-border.md)** – The color of a control's border when the user keeps the mouse pointer on that control.

**[HoverColor](../properties/properties-color-border.md)** – The color of the text in a control when the user keeps the mouse pointer on it.

**[HoverFill](../properties/properties-color-border.md)** – The background color of a control when the user keeps the mouse pointer on it.

**[Italic](../properties/properties-text.md)** – Whether the text in a control is italic.

**[LineHeight](../properties/properties-text.md)** – The distance between, for example, lines of text or items in a list.

**MaxLength** – The number of characters that the user can type into a text-input control.

**Mode** – The control is in **SingleLine**, **MultiLine**, or **Password** mode.

**[OnChange](../properties/properties-core.md)** – How the app responds when the user changes the value of a control (for example, by adjusting a slider).

**[OnSelect](../properties/properties-core.md)** – How the app responds when the user taps or clicks a control.

**[PaddingBottom](../properties/properties-size-location.md)** – The distance between text in a control and the bottom edge of that control.

**[PaddingLeft](../properties/properties-size-location.md)** – The distance between text in a control and the left edge of that control.

**[PaddingRight](../properties/properties-size-location.md)** – The distance between text in a control and the right edge of that control.

**[PaddingTop](../properties/properties-size-location.md)** – The distance between text in a control and the top edge of that control.

**[PressedBorderColor](../properties/properties-color-border.md)** – The color of a control's border when the user taps or clicks that control.

**[PressedColor](../properties/properties-color-border.md)** – The color of text in a control when the user taps or clicks that control.

**[PressedFill](../properties/properties-color-border.md)** – The background color of a control when the user taps or clicks that control.

**[RadiusBottomLeft](../properties/properties-size-location.md)** – The degree to which the bottom-left corner of a control is rounded.

**[RadiusBottomRight](../properties/properties-size-location.md)** – The degree to which the bottom-right corner of a control is rounded.

**[RadiusTopLeft](../properties/properties-size-location.md)** – The degree to which the top-left corner of a control is rounded.

**[RadiusTopRight](../properties/properties-size-location.md)** – The degree to which the top-right corner of a control is rounded.

**[Reset](../properties/properties-core.md)** – Whether a control reverts to its default value.

**[Size](../properties/properties-text.md)** – The font size of the text that appears on a control.

**[Strikethrough](../properties/properties-text.md)** – Whether a line appears through the text that appears on a control.

**[Tooltip](../properties/properties-core.md)** – Explanatory text that appears when the user hovers over a control.

**[Underline](../properties/properties-text.md)** – Whether a line appears under the text that appears on a control.

**[Visible](../properties/properties-core.md)** – Whether a control appears or is hidden.

**[Width](../properties/properties-size-location.md)** – The distance between a control's left and right edges.

**[X](../properties/properties-size-location.md)** – The distance between the left edge of a control and the left edge of the screen.

**[Y](../properties/properties-size-location.md)** – The distance between the top edge of a control and the top edge of the screen.

## Related functions ##

[**DateTimeValue**( *String* )](function-datevalue-timevalue.md)

## Examples ##

### Collect data ###
1. Add two text-input controls, and name them **inputFirst** and **inputLast**.

	Don't know how to [add, name, and configure a control](add-configure-controls.md)?

1. Add a button, set its **Text** property to **Add**, and set its **OnSelect** property to this formula:<br>
**Collect(Names, {FirstName:inputFirst.Text, LastName:inputLast.Text})**

	Want more information about the [**Collect** function](function-clear-collect-clearcollect.md) or [other functions](formula-reference.md)?

1. Add a text gallery in portrait/vertical orientation, set its **Items** property to **Names**, and set the **Text** property of **Subtitle1** to **ThisItem.FirstName**.

1. (optional) In the template gallery, delete the bottom text box, named **Body1**, and set the **TemplateSize** property of the gallery to **80**.

1. Press F5, type a string of text into **inputFirst** and **inputLast**, and then click or tap the **Add** button.

1. (optional) Add more names to the collection, and then press Esc to return to the default workspace.

### Prompt for a password ###
1. Add a text-input control, name it **inputPassword**, and set its **Mode** property to **Password**.

1. Add a text box, and set its **Text** property to this formula:<br>
**If(inputPassword.Text = "P@ssw0rd", "Access granted", "Access denied")**

	Want more information about the [**If** function](function-if.md) or [other functions](formula-reference.md)?

1. Press F5, and then type **P@ssw0rd** in **inputPassword**.

	When you finish typing the password, the text box stops showing **Access denied** and starts to show **Access granted**.

1. To return to the default workspace, press Esc.

1. (optional) Add a control such as an arrow, configure it to navigate to another screen, and show it only after the user types the password.

1. (optional) Add a button, configure its **Text** property to show **Sign in**, add a timer, and disable the input-text control for a certain amount of time if the user types the wrong password and then clicks or taps the **Sign in** button.