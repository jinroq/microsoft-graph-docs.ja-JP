---
title: objectMapping リソースの種類
description: どのように特定のオブジェクト同期する必要があるソース ディレクトリからコピー先のディレクトリを定義します。 ソース ディレクトリ内のオブジェクトのコピー先のディレクトリ内のオブジェクトとの照合方法を定義する具体的には、どのような (もしあれば) フィルターのスコープを使用するかどうかは、特定のオブジェクトを準備して、変換からのオブジェクトの属性がどのようにする必要がありますかを決定する必要があります先のディレクトリにソースです。
localization_priority: Normal
ms.openlocfilehash: 274d401c28abc25d904c259b00a673f3c0a53888
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526915"
---
# <a name="objectmapping-resource-type"></a><span data-ttu-id="d69cf-104">objectMapping リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d69cf-104">objectMapping resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d69cf-105">どのように特定のオブジェクト同期する必要があるソース ディレクトリからコピー先のディレクトリを定義します。</span><span class="sxs-lookup"><span data-stu-id="d69cf-105">Defines how a given object should be synchronized from source directory to target directory.</span></span> <span data-ttu-id="d69cf-106">ソース ディレクトリ内のオブジェクトのコピー先のディレクトリ内のオブジェクトとの照合方法を定義する具体的には、どのような (もしあれば) フィルターのスコープを使用するかどうかは、特定のオブジェクトを準備して、変換からのオブジェクトの属性がどのようにする必要がありますかを決定する必要があります先のディレクトリにソースです。</span><span class="sxs-lookup"><span data-stu-id="d69cf-106">In particular, it defines how object in source directory should be matched with an object in target directory, what (if any) scoping filters should be used to decide if we want to provision a given object, and how object attributes should be transformed going from source to target directory.</span></span>

<span data-ttu-id="d69cf-107">オブジェクトのマッピングでは、[同期ルール](synchronization-synchronizationrule.md)の主な一部であるし、[同期スキーマ](synchronization-synchronizationschema.md)の一部として更新されます。</span><span class="sxs-lookup"><span data-stu-id="d69cf-107">Object mappings are the main part of the [synchronization rule](synchronization-synchronizationrule.md) and are updated as part of [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d69cf-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d69cf-108">Properties</span></span>

| <span data-ttu-id="d69cf-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d69cf-109">Property</span></span>      | <span data-ttu-id="d69cf-110">型</span><span class="sxs-lookup"><span data-stu-id="d69cf-110">Type</span></span>      | <span data-ttu-id="d69cf-111">説明</span><span class="sxs-lookup"><span data-stu-id="d69cf-111">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="d69cf-112">attributeMappings</span><span class="sxs-lookup"><span data-stu-id="d69cf-112">attributeMappings</span></span>  |<span data-ttu-id="d69cf-113">[attributeMapping](synchronization-attributemapping.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d69cf-113">[attributeMapping](synchronization-attributemapping.md) collection</span></span>    | <span data-ttu-id="d69cf-114">属性のマッピングは、ソース オブジェクトからターゲット オブジェクトとフローの方法にマップする属性を定義します。</span><span class="sxs-lookup"><span data-stu-id="d69cf-114">Attribute mappings define which attributes to map from the source object into the target object and how they should flow.</span></span> <span data-ttu-id="d69cf-115">元のソースの値の変換をサポートするために多くの機能を利用できます。</span><span class="sxs-lookup"><span data-stu-id="d69cf-115">A number of functions are available to support the transformation of the original source values.</span></span>|
|<span data-ttu-id="d69cf-116">enabled</span><span class="sxs-lookup"><span data-stu-id="d69cf-116">enabled</span></span>        |<span data-ttu-id="d69cf-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69cf-117">Boolean</span></span>    |<span data-ttu-id="d69cf-118">`true`、このオブジェクトのマッピングが同期中に処理されます。</span><span class="sxs-lookup"><span data-stu-id="d69cf-118">When `true`, this object mapping will be processed during synchronization.</span></span> <span data-ttu-id="d69cf-119">`false`、このオブジェクトのマッピングはスキップされます。</span><span class="sxs-lookup"><span data-stu-id="d69cf-119">When `false`, this object mapping will be skipped.</span></span>|
|<span data-ttu-id="d69cf-120">flowTypes</span><span class="sxs-lookup"><span data-stu-id="d69cf-120">flowTypes</span></span>      |<span data-ttu-id="d69cf-121">objectFlowType</span><span class="sxs-lookup"><span data-stu-id="d69cf-121">objectFlowType</span></span>    |<span data-ttu-id="d69cf-122">どのフローの種類では、このオブジェクトのマッピングは有効です。</span><span class="sxs-lookup"><span data-stu-id="d69cf-122">Which flow types are enabled for this object mapping.</span></span> <span data-ttu-id="d69cf-123">`Add`コピー先のディレクトリに新しいオブジェクトを作成`Update`、既存のオブジェクトを変更し、`Delete`既存のユーザーを deprovisions。</span><span class="sxs-lookup"><span data-stu-id="d69cf-123">`Add` creates new objects in the target directory, `Update` modifies existing objects, and `Delete` deprovisions existing users.</span></span> <span data-ttu-id="d69cf-124">既定値は `Add, Update, Delete` です。</span><span class="sxs-lookup"><span data-stu-id="d69cf-124">The default is `Add, Update, Delete`.</span></span> |
|<span data-ttu-id="d69cf-125">metadata</span><span class="sxs-lookup"><span data-stu-id="d69cf-125">metadata</span></span>       |<span data-ttu-id="d69cf-126">metadataEntry コレクション</span><span class="sxs-lookup"><span data-stu-id="d69cf-126">metadataEntry collection</span></span>    |<span data-ttu-id="d69cf-127">プロパティをさらに拡張します。</span><span class="sxs-lookup"><span data-stu-id="d69cf-127">Additional extension properties.</span></span> <span data-ttu-id="d69cf-128">明示的に記載されている、しない限り、メタデータの値を変更できませんする必要があります。</span><span class="sxs-lookup"><span data-stu-id="d69cf-128">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="d69cf-129">name</span><span class="sxs-lookup"><span data-stu-id="d69cf-129">name</span></span>           |<span data-ttu-id="d69cf-130">String</span><span class="sxs-lookup"><span data-stu-id="d69cf-130">String</span></span>     |<span data-ttu-id="d69cf-131">オブジェクトのマッピングのわかりやすい名前です。</span><span class="sxs-lookup"><span data-stu-id="d69cf-131">Human-friendly name of the object mapping.</span></span>|
|<span data-ttu-id="d69cf-132">scope</span><span class="sxs-lookup"><span data-stu-id="d69cf-132">scope</span></span>          |[<span data-ttu-id="d69cf-133">filter</span><span class="sxs-lookup"><span data-stu-id="d69cf-133">filter</span></span>](synchronization-filter.md)     |<span data-ttu-id="d69cf-134">特定のオブジェクトを準備する必要があるかどうかを決定する際に使用するフィルターを定義します。</span><span class="sxs-lookup"><span data-stu-id="d69cf-134">Defines a filter to be used when deciding whether a given object should be provisioned.</span></span> <span data-ttu-id="d69cf-135">たとえば、米国内にあるユーザーのみを提供する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d69cf-135">For example, you might want to only provision users that are located in the US.</span></span>|
|<span data-ttu-id="d69cf-136">sourceObjectName</span><span class="sxs-lookup"><span data-stu-id="d69cf-136">sourceObjectName</span></span>           |<span data-ttu-id="d69cf-137">String</span><span class="sxs-lookup"><span data-stu-id="d69cf-137">String</span></span>     |<span data-ttu-id="d69cf-138">ソース ディレクトリ内のオブジェクトの名前です。</span><span class="sxs-lookup"><span data-stu-id="d69cf-138">Name of the object in the source directory.</span></span> <span data-ttu-id="d69cf-139">ソース[ディレクトリの定義](synchronization-directorydefinition.md)からオブジェクトの名前と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d69cf-139">Must match the object name from the source [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="d69cf-140">targetObjectName</span><span class="sxs-lookup"><span data-stu-id="d69cf-140">targetObjectName</span></span>           |<span data-ttu-id="d69cf-141">String</span><span class="sxs-lookup"><span data-stu-id="d69cf-141">String</span></span>     |<span data-ttu-id="d69cf-142">ターゲット ディレクトリ内のオブジェクトの名前です。</span><span class="sxs-lookup"><span data-stu-id="d69cf-142">Name of the object in target directory.</span></span> <span data-ttu-id="d69cf-143">ターゲット[ディレクトリの定義](synchronization-directorydefinition.md)からオブジェクトの名前と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d69cf-143">Must match the object name from the target [directory definition](synchronization-directorydefinition.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d69cf-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d69cf-144">JSON representation</span></span>

<span data-ttu-id="d69cf-145">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d69cf-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.objectMapping"
}-->

```json
{
  "attributeMappings": [{"@odata.type": "microsoft.graph.attributeMapping"}],
  "enabled": true,
  "flowTypes": "String",
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "name": "String",
  "scope": {"@odata.type": "microsoft.graph.filter"},
  "sourceObjectName": "String",
  "targetObjectName": "String"
}
```

## <a name="json-example"></a><span data-ttu-id="d69cf-146">JSON の例</span><span class="sxs-lookup"><span data-stu-id="d69cf-146">JSON Example</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.objectMapping"
}-->

```json
{
    "attributeMappings": [
        {
            "defaultValue": "True",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "Not([IsSoftDeleted])",
                "name": "Not",
                "parameters": [
                    {
                        "key": "source",
                        "value": {
                            "expression": "[IsSoftDeleted]",
                            "name": "IsSoftDeleted",
                            "parameters": [],
                            "type": "Attribute"
                        }
                    }
                ],
                "type": "Function"
            },
            "targetAttributeName": "IsActive"
        },
        {
            "defaultValue": null,
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "Mid([userPrincipalName], 1, 8)",
                "name": "Mid",
                "parameters": [
                    {
                        "key": "source",
                        "value": {
                            "expression": "[userPrincipalName]",
                            "name": "userPrincipalName",
                            "parameters": [],
                            "type": "Attribute"
                        }
                    },
                    {
                        "key": "start",
                        "value": {
                            "expression": "\"1\"",
                            "name": "1",
                            "parameters": [],
                            "type": "Constant"
                        }
                    },
                    {
                        "key": "length",
                        "value": {
                            "expression": "\"8\"",
                            "name": "8",
                            "parameters": [],
                            "type": "Constant"
                        }
                    }
                ],
                "type": "Function"
            },
            "targetAttributeName": "Alias"
        },
        {
            "defaultValue": null,
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "[mail]",
                "name": "mail",
                "parameters": [],
                "type": "Attribute"
            },
            "targetAttributeName": "Email"
        },
        {
            "defaultValue": "ISO-8859-1",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "EmailEncodingKey"
        },
        {
            "defaultValue": "en_US",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "LanguageLocaleKey"
        },
        {
            "defaultValue": null,
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "[givenName]",
                "name": "givenName",
                "parameters": [],
                "type": "Attribute"
            },
            "targetAttributeName": "FirstName"
        },
        {
            "defaultValue": ".",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "[surname]",
                "name": "surname",
                "parameters": [],
                "type": "Attribute"
            },
            "targetAttributeName": "LastName"
        },
        {
            "defaultValue": "en_US",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "Replace([preferredLanguage], \"-\", , , \"_\", , )",
                "name": "Replace",
                "parameters": [
                    {
                        "key": "source",
                        "value": {
                            "expression": "[preferredLanguage]",
                            "name": "preferredLanguage",
                            "parameters": [],
                            "type": "Attribute"
                        }
                    },
                    {
                        "key": "Find",
                        "value": {
                            "expression": "\"-\"",
                            "name": "-",
                            "parameters": [],
                            "type": "Constant"
                        }
                    },
                    {
                        "key": "Replacement",
                        "value": {
                            "expression": "\"_\"",
                            "name": "_",
                            "parameters": [],
                            "type": "Constant"
                        }
                    }
                ],
                "type": "Function"
            },
            "targetAttributeName": "LocaleSidKey"
        },
        {
            "defaultValue": "Chatter Free User",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": {
                "expression": "SingleAppRoleAssignment([appRoleAssignments])",
                "name": "SingleAppRoleAssignment",
                "parameters": [
                    {
                        "key": "source",
                        "value": {
                            "expression": "[appRoleAssignments]",
                            "name": "appRoleAssignments",
                            "parameters": [],
                            "type": "Attribute"
                        }
                    }
                ],
                "type": "Function"
            },
            "targetAttributeName": "ProfileName"
        },
        {
            "defaultValue": "America/Los_Angeles",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "TimeZoneSidKey"
        },
        {
            "defaultValue": null,
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 1,
            "source": {
                "expression": "[userPrincipalName]",
                "name": "userPrincipalName",
                "parameters": [],
                "type": "Attribute"
            },
            "targetAttributeName": "Username"
        },
        {
            "defaultValue": "False",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "UserPermissionsCallCenterAutoLogin"
        },
        {
            "defaultValue": "False",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "UserPermissionsMarketingUser"
        },
        {
            "defaultValue": "False",
            "exportMissingReferences": false,
            "flowBehavior": "FlowWhenChanged",
            "flowType": "Always",
            "matchingPriority": 0,
            "source": null,
            "targetAttributeName": "UserPermissionsOfflineUser"
        }
    ],
    "enabled": true,
    "flowTypes": "Add, Update, Delete",
    "metadata": [
        {
            "key": "IsCustomerDefined",
            "value": "false"
        },
        {
            "key": "DisableMonitoringForChanges",
            "value": "false"
        },
        {
            "key": "Disposition",
            "value": "\"Normal\""
        },
        {
            "key": "ExcludeFromReporting",
            "value": "false"
        },
        {
            "key": "EscrowBehavior",
            "value": "\"Default\""
        },
        {
            "key": "Unsynchronized",
            "value": "false"
        }
    ],
    "name": "Synchronize Azure Active Directory Users to salesforce.com",
    "scope": null,
    "sourceObjectName": "User",
    "targetObjectName": "User"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "objectMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-objectmapping.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
