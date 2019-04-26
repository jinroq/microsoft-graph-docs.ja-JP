---
title: directorydefinition リソースの種類
description: ディレクトリとそのオブジェクトに関する同期エンジン情報を提供します。 このリソースは、同期エンジンに対して、たとえば、ディレクトリには、**ユーザー**と**グループ**という名前のオブジェクト、これらのオブジェクトに対してサポートされている属性、およびそれらの属性の種類を示します。 オブジェクトと属性を同期ルールおよびオブジェクトマッピングに参加させるには、それらをディレクトリ定義の一部として定義する必要があります。
localization_priority: Normal
ms.openlocfilehash: 8e622edef39eec5476015ef5e22c5fe9697e0daa
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342924"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="25e4a-105">directorydefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="25e4a-105">directoryDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25e4a-106">ディレクトリとそのオブジェクトに関する同期エンジン情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="25e4a-106">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="25e4a-107">このリソースは、同期エンジンに対して、たとえば、ディレクトリには、**ユーザー**と**グループ**という名前のオブジェクト、これらのオブジェクトに対してサポートされている属性、およびそれらの属性の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="25e4a-107">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="25e4a-108">オブジェクトと属性を[同期ルール](synchronization-synchronizationrule.md)および[オブジェクトマッピング](synchronization-objectmapping.md)に参加させるには、それらをディレクトリ定義の一部として定義する必要があります。</span><span class="sxs-lookup"><span data-stu-id="25e4a-108">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="25e4a-109">通常、[同期テンプレート](synchronization-synchronizationtemplate.md)の一部として提供される既定の[同期スキーマ](synchronization-synchronizationschema.md)は、そのディレクトリに最もよく使用されるオブジェクトと属性を定義します。</span><span class="sxs-lookup"><span data-stu-id="25e4a-109">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="25e4a-110">ただし、ディレクトリでカスタム属性の追加がサポートされている場合は、独自のカスタムオブジェクトまたは属性を使用して、既定の定義を拡張することもできます。</span><span class="sxs-lookup"><span data-stu-id="25e4a-110">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="25e4a-111">詳細については、「[カスタム属性を使用して同期を構成する](synchronization-configure-with-custom-target-attributes.md)」および「 [configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="25e4a-111">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="25e4a-112">ディレクトリ定義は、[同期スキーマ](synchronization-synchronizationschema.md)の一部として更新されます。</span><span class="sxs-lookup"><span data-stu-id="25e4a-112">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="25e4a-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25e4a-113">Properties</span></span>

| <span data-ttu-id="25e4a-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25e4a-114">Property</span></span>      | <span data-ttu-id="25e4a-115">型</span><span class="sxs-lookup"><span data-stu-id="25e4a-115">Type</span></span>      | <span data-ttu-id="25e4a-116">説明</span><span class="sxs-lookup"><span data-stu-id="25e4a-116">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="25e4a-117">id</span><span class="sxs-lookup"><span data-stu-id="25e4a-117">id</span></span>           |<span data-ttu-id="25e4a-118">String</span><span class="sxs-lookup"><span data-stu-id="25e4a-118">String</span></span>     |<span data-ttu-id="25e4a-119">ディレクトリ識別子。</span><span class="sxs-lookup"><span data-stu-id="25e4a-119">Directory identifier.</span></span> <span data-ttu-id="25e4a-120">null 許容型ではありません。</span><span class="sxs-lookup"><span data-stu-id="25e4a-120">Not nullable.</span></span>|
|<span data-ttu-id="25e4a-121">metadata</span><span class="sxs-lookup"><span data-stu-id="25e4a-121">metadata</span></span>       |<span data-ttu-id="25e4a-122">metadataentry コレクション</span><span class="sxs-lookup"><span data-stu-id="25e4a-122">metadataEntry collection</span></span>    |<span data-ttu-id="25e4a-123">追加の拡張機能のプロパティ。</span><span class="sxs-lookup"><span data-stu-id="25e4a-123">Additional extension properties.</span></span> <span data-ttu-id="25e4a-124">明示的に記述されていない限り、メタデータ値は変更しないでください。</span><span class="sxs-lookup"><span data-stu-id="25e4a-124">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="25e4a-125">name</span><span class="sxs-lookup"><span data-stu-id="25e4a-125">name</span></span>           |<span data-ttu-id="25e4a-126">String</span><span class="sxs-lookup"><span data-stu-id="25e4a-126">String</span></span>     |<span data-ttu-id="25e4a-127">ディレクトリの名前。</span><span class="sxs-lookup"><span data-stu-id="25e4a-127">Name of the directory.</span></span> <span data-ttu-id="25e4a-128">[同期スキーマ](synchronization-synchronizationschema.md)内で一意である必要があります。</span><span class="sxs-lookup"><span data-stu-id="25e4a-128">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="25e4a-129">null 許容型ではありません。</span><span class="sxs-lookup"><span data-stu-id="25e4a-129">Not nullable.</span></span>|
|<span data-ttu-id="25e4a-130">対象</span><span class="sxs-lookup"><span data-stu-id="25e4a-130">objects</span></span>        |<span data-ttu-id="25e4a-131">[objectdefinition](synchronization-objectdefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="25e4a-131">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="25e4a-132">ディレクトリでサポートされているオブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="25e4a-132">Collection of objects supported by the directory.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="25e4a-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="25e4a-133">JSON representation</span></span>

<span data-ttu-id="25e4a-134">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="25e4a-134">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-example"></a><span data-ttu-id="25e4a-135">JSON の例</span><span class="sxs-lookup"><span data-stu-id="25e4a-135">JSON Example</span></span>

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
  "suppressions": []
}
-->
