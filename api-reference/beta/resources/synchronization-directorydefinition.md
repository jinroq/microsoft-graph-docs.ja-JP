---
title: directoryDefinition リソースの種類
description: ディレクトリとそのオブジェクトの同期エンジンに関する情報を提供します。 このリソースは、同期エンジンなどのディレクトリが**ユーザー**と**グループ**、それらのオブジェクトとそれらの属性の型の属性はサポートされてをという名前のオブジェクトを持っています。 同期化規則とオブジェクトのマッピングに参加するオブジェクトおよび属性の順序で、ディレクトリの定義の一部としてこれらに定義しなければなりません。
localization_priority: Normal
ms.openlocfilehash: 22ba4a7f3b5b5d3154ec6b3f5d42bd6f1b8f09d7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508126"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="aff02-105">directoryDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aff02-105">directoryDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aff02-106">ディレクトリとそのオブジェクトの同期エンジンに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="aff02-106">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="aff02-107">このリソースは、同期エンジンなどのディレクトリが**ユーザー**と**グループ**、それらのオブジェクトとそれらの属性の型の属性はサポートされてをという名前のオブジェクトを持っています。</span><span class="sxs-lookup"><span data-stu-id="aff02-107">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="aff02-108">[同期化規則](synchronization-synchronizationrule.md)と[オブジェクトのマッピング](synchronization-objectmapping.md)に参加するオブジェクトおよび属性の順序で、ディレクトリの定義の一部としてこれらに定義しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="aff02-108">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="aff02-109">一般に、[同期のテンプレート](synchronization-synchronizationtemplate.md)の一部として提供されている既定の[スキーマの同期](synchronization-synchronizationschema.md)では、最も一般的に使用されるオブジェクトおよびそのディレクトリの属性を定義します。</span><span class="sxs-lookup"><span data-stu-id="aff02-109">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="aff02-110">ただし、ディレクトリでは、カスタム属性の追加をサポートする場合、独自のカスタム オブジェクトまたは属性の既定の定義を展開します。</span><span class="sxs-lookup"><span data-stu-id="aff02-110">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="aff02-111">詳細については、[カスタム属性を使用して同期を構成](synchronization-configure-with-custom-target-attributes.md)し、[ディレクトリの拡張属性を使用して構成の同期](synchronization-configure-with-directory-extension-attributes.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aff02-111">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="aff02-112">ディレクトリの定義は、[同期スキーマ](synchronization-synchronizationschema.md)の一部として更新されます。</span><span class="sxs-lookup"><span data-stu-id="aff02-112">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="aff02-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aff02-113">Properties</span></span>

| <span data-ttu-id="aff02-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aff02-114">Property</span></span>      | <span data-ttu-id="aff02-115">型</span><span class="sxs-lookup"><span data-stu-id="aff02-115">Type</span></span>      | <span data-ttu-id="aff02-116">説明</span><span class="sxs-lookup"><span data-stu-id="aff02-116">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="aff02-117">id</span><span class="sxs-lookup"><span data-stu-id="aff02-117">id</span></span>           |<span data-ttu-id="aff02-118">String</span><span class="sxs-lookup"><span data-stu-id="aff02-118">String</span></span>     |<span data-ttu-id="aff02-119">ディレクトリの識別子です。</span><span class="sxs-lookup"><span data-stu-id="aff02-119">Directory identifier.</span></span> <span data-ttu-id="aff02-120">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="aff02-120">Not nullable.</span></span>|
|<span data-ttu-id="aff02-121">metadata</span><span class="sxs-lookup"><span data-stu-id="aff02-121">metadata</span></span>       |<span data-ttu-id="aff02-122">metadataEntry コレクション</span><span class="sxs-lookup"><span data-stu-id="aff02-122">metadataEntry collection</span></span>    |<span data-ttu-id="aff02-123">プロパティをさらに拡張します。</span><span class="sxs-lookup"><span data-stu-id="aff02-123">Additional extension properties.</span></span> <span data-ttu-id="aff02-124">明示的に記載されている、しない限り、メタデータの値を変更できませんする必要があります。</span><span class="sxs-lookup"><span data-stu-id="aff02-124">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="aff02-125">name</span><span class="sxs-lookup"><span data-stu-id="aff02-125">name</span></span>           |<span data-ttu-id="aff02-126">String</span><span class="sxs-lookup"><span data-stu-id="aff02-126">String</span></span>     |<span data-ttu-id="aff02-127">ディレクトリの名前です。</span><span class="sxs-lookup"><span data-stu-id="aff02-127">Name of the directory.</span></span> <span data-ttu-id="aff02-128">[同期スキーマ](synchronization-synchronizationschema.md)内で一意である必要があります。</span><span class="sxs-lookup"><span data-stu-id="aff02-128">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="aff02-129">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="aff02-129">Not nullable.</span></span>|
|<span data-ttu-id="aff02-130">オブジェクト</span><span class="sxs-lookup"><span data-stu-id="aff02-130">objects</span></span>        |<span data-ttu-id="aff02-131">[objectDefinition](synchronization-objectdefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="aff02-131">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="aff02-132">ディレクトリでサポートされているオブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="aff02-132">Collection of objects supported by the directory.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aff02-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aff02-133">JSON representation</span></span>

<span data-ttu-id="aff02-134">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="aff02-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryDefinition"
}-->

```json
{
  "id": "String",
  "name": "String",
  "objects": [{"@odata.type": "microsoft.graph.objectDefinition"}]
}

```

## <a name="json-example"></a><span data-ttu-id="aff02-135">JSON の例</span><span class="sxs-lookup"><span data-stu-id="aff02-135">JSON Example</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryDefinition"
}-->

```json
{
    "id": "8ffa6169-f354-4751-9b77-9c00765be92d",
    "name": "salesforce.com",
    "objects": [
        {
            "attributes": [
                {
                    "anchor": true,
                    "name": "Id",
                    "type": "String"
                },
                {
                    "name": "IsActive",
                    "required": true,
                    "type": "Boolean"
                },
                {
                    "mutability": "ReadWrite",
                    "name": "Alias",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "CompanyName",
                    "type": "String"
                },
                {
                    "name": "CommunityNickname",
                    "type": "String"
                },
                {
                    "name": "Email",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "EmailEncodingKey",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "LanguageLocaleKey",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "FirstName",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "LastName",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "LocaleSidKey",
                    "required": true,
                    "type": "String"
                },
                {
                    "metadata": [
                        {
                            "key": "LinkTypeName",
                            "value": "PermissionSetAssignment"
                        },
                        {
                            "key": "LinkPropertyNames",
                            "value": "[\"PermissionSetId\"]"
                        }
                    ],
                    "name": "PermissionSets",
                    "referencedObjects": [
                        {
                            "referencedObjectName": "PermissionSet"
                        }
                    ],
                    "type": "Reference"
                },
                {
                    "name": "ProfileId",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "ProfileName",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "TimeZoneSidKey",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "Username",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "UserPermissionsCallCenterAutoLogin",
                    "required": true,
                    "type": "Boolean"
                },
                {
                    "name": "UserPermissionsMarketingUser",
                    "required": true,
                    "type": "Boolean"
                },
                {
                    "name": "Street",
                    "type": "String"
                },
                {
                    "name": "City",
                    "type": "String"
                },
                {
                    "name": "Division",
                    "type": "String"
                },
                {
                    "name": "EmployeeNumber",
                    "type": "String"
                },
                {
                    "name": "State",
                    "type": "String"
                },
                {
                    "name": "PostalCode",
                    "type": "String"
                },
                {
                    "name": "Country",
                    "type": "String"
                },
                {
                    "name": "Department",
                    "type": "String"
                },
                {
                    "name": "MobilePhone",
                    "type": "String"
                },
                {
                    "name": "Phone",
                    "type": "String"
                },
                {
                    "name": "Title",
                    "type": "String"
                },
                {
                    "name": "FederationIdentifier",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "ManagerId",
                    "referencedObjects": [
                        {
                            "referencedObjectName": "User"
                        }
                    ],
                    "type": "Reference"
                },
                {
                    "name": "UserRoleId",
                    "referencedObjects": [
                        {
                            "referencedObjectName": "UserRole"
                        }
                    ],
                    "type": "Reference"
                }
            ],
            "metadata": [
                {
                    "key": "IsSoftDeletionSupported",
                    "value": "false"
                },
                {
                    "key": "ConnectorDataStorageRequired",
                    "value": "false"
                },
                {
                    "key": "IsSynchronizeAllSupported",
                    "value": "false"
                }
            ],
            "name": "User"
        }
    ],
    "metadata": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-directorydefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
