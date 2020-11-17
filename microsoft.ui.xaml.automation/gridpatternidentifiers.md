---
-api-id: T:Microsoft.UI.Xaml.Automation.GridPatternIdentifiers
-api-type: winrt class
---

<!-- Class syntax.
public class GridPatternIdentifiers : Windows.UI.Xaml.Automation.IGridPatternIdentifiers
-->

# Microsoft.UI.Xaml.Automation.GridPatternIdentifiers

## -description
Contains values used as identifiers by [IGridProvider](../microsoft.ui.xaml.automation.provider/igridprovider.md).

## -remarks
Classes such as GridPatternIdentifiers are the identifiers for the Windows Runtime implementation of a common provider pattern for Microsoft UI Automation. You might use these identifiers if you are implementing a Windows Runtime custom automation peer that reports support for [IGridProvider](../microsoft.ui.xaml.automation.provider/igridprovider.md) in its [GetPattern](/uwp/api/windows.ui.xaml.automation.peers.automationpeer.getpattern(windows.ui.xaml.automation.peers.patterninterface)) implementation. These identifiers are needed for the [RaisePropertyChangedEvent](/uwp/api/windows.ui.xaml.automation.peers.automationpeer.raisepropertychangedevent(windows.ui.xaml.automation.automationproperty,system.object,system.object)) calls that you make from control code that references your own peer, or for [FindItemByProperty](/uwp/api/windows.ui.xaml.automation.provider.iitemcontainerprovider.finditembyproperty(windows.ui.xaml.automation.provider.irawelementprovidersimple,windows.ui.xaml.automation.automationproperty,system.object)) in an items container peer.

This same pattern is usually exposed to clients in a different way, depending on which technology they use to implement the client and examine the Microsoft UI Automation tree. [IGridProvider](../microsoft.ui.xaml.automation.provider/igridprovider.md) is also presented as a Component Object Model (COM) interface.

## -examples

## -see-also
[IGridProvider](../microsoft.ui.xaml.automation.provider/igridprovider.md), [Control patterns and interfaces](/windows/uwp/accessibility/control-patterns-and-interfaces), [Custom automation peers](/windows/uwp/accessibility/custom-automation-peers)