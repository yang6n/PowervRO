# Remove-vROWorkflow

## SYNOPSIS
    
Remove a vRO Workflow

## SYNTAX
 Remove-vROWorkflow [-Id] <String[]> [-Force] [-WhatIf] [-Confirm] [<CommonParameters>]    

## DESCRIPTION

Remove a vRO Workflow

## PARAMETERS


### Id

Workflow ID

* Required: true
* Position: 1
* Default value: 
* Accept pipeline input: true (ByValue, ByPropertyName)

### Force

If the workflow is referenced by some other workflows, or is running, it is considered to be 'in use' and the delete 
operation will fail, unless the 'force' option is provided.

* Required: false
* Position: named
* Default value: False
* Accept pipeline input: false

### WhatIf


* Required: false
* Position: named
* Default value: 
* Accept pipeline input: false

### Confirm


* Required: false
* Position: named
* Default value: 
* Accept pipeline input: false

## INPUTS

System.String.
Switch

## OUTPUTS

None

## EXAMPLES
```
-------------------------- EXAMPLE 1 --------------------------

PS C:\>Remove-vROWorkflow -Id "3f92d2dc-a9fa-4323-900b-ef97196184ea"







-------------------------- EXAMPLE 2 --------------------------

PS C:\>Get-vROWorkflow -Name Test01 | Remove-vROWorkflow -Confirm:$false
```

