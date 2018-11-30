---
title: directoryDefinition リソースの種類
description: ディレクトリとそのオブジェクトの同期エンジンに関する情報を提供します。 このリソースは、同期エンジンなどのディレクトリが**ユーザー**と**グループ**、それらのオブジェクトとそれらの属性の型の属性はサポートされてをという名前のオブジェクトを持っています。 同期化規則とオブジェクトのマッピングに参加するオブジェクトおよび属性の順序で、ディレクトリの定義の一部としてこれらに定義しなければなりません。
ms.openlocfilehash: ddc32237efc18d43da23d815aea00ee01b2650be
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074013"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="30e52-105">directoryDefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="30e52-105">directoryDefinition resource type</span></span>

> <span data-ttu-id="30e52-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="30e52-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30e52-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="30e52-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="30e52-108">ディレクトリとそのオブジェクトの同期エンジンに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="30e52-108">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="30e52-109">このリソースは、同期エンジンなどのディレクトリが**ユーザー**と**グループ**、それらのオブジェクトとそれらの属性の型の属性はサポートされてをという名前のオブジェクトを持っています。</span><span class="sxs-lookup"><span data-stu-id="30e52-109">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="30e52-110">[同期化規則](synchronization-synchronizationrule.md)と[オブジェクトのマッピング](synchronization-objectmapping.md)に参加するオブジェクトおよび属性の順序で、ディレクトリの定義の一部としてこれらに定義しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="30e52-110">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="30e52-111">一般に、[同期のテンプレート](synchronization-synchronizationtemplate.md)の一部として提供されている既定の[スキーマの同期](synchronization-synchronizationschema.md)では、最も一般的に使用されるオブジェクトおよびそのディレクトリの属性を定義します。</span><span class="sxs-lookup"><span data-stu-id="30e52-111">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="30e52-112">ただし、ディレクトリでは、カスタム属性の追加をサポートする場合、独自のカスタム オブジェクトまたは属性の既定の定義を展開します。</span><span class="sxs-lookup"><span data-stu-id="30e52-112">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="30e52-113">詳細については、[カスタム属性を使用して同期を構成](synchronization-configure-with-custom-target-attributes.md)し、[ディレクトリの拡張属性を使用して構成の同期](synchronization-configure-with-directory-extension-attributes.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="30e52-113">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="30e52-114">ディレクトリの定義は、[同期スキーマ](synchronization-synchronizationschema.md)の一部として更新されます。</span><span class="sxs-lookup"><span data-stu-id="30e52-114">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="30e52-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30e52-115">Properties</span></span>

| <span data-ttu-id="30e52-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30e52-116">Property</span></span>      | <span data-ttu-id="30e52-117">型</span><span class="sxs-lookup"><span data-stu-id="30e52-117">Type</span></span>      | <span data-ttu-id="30e52-118">説明</span><span class="sxs-lookup"><span data-stu-id="30e52-118">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="30e52-119">id</span><span class="sxs-lookup"><span data-stu-id="30e52-119">id</span></span>           |<span data-ttu-id="30e52-120">String</span><span class="sxs-lookup"><span data-stu-id="30e52-120">String</span></span>     |<span data-ttu-id="30e52-121">ディレクトリの識別子です。</span><span class="sxs-lookup"><span data-stu-id="30e52-121">Directory identifier.</span></span> <span data-ttu-id="30e52-122">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="30e52-122">Not nullable.</span></span>|
|<span data-ttu-id="30e52-123">metadata</span><span class="sxs-lookup"><span data-stu-id="30e52-123">metadata</span></span>       |<span data-ttu-id="30e52-124">metadataEntry コレクション</span><span class="sxs-lookup"><span data-stu-id="30e52-124">metadataEntry collection</span></span>    |<span data-ttu-id="30e52-125">プロパティをさらに拡張します。</span><span class="sxs-lookup"><span data-stu-id="30e52-125">Additional extension properties.</span></span> <span data-ttu-id="30e52-126">明示的に記載されている、しない限り、メタデータの値を変更できませんする必要があります。</span><span class="sxs-lookup"><span data-stu-id="30e52-126">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="30e52-127">名前</span><span class="sxs-lookup"><span data-stu-id="30e52-127">name</span></span>           |<span data-ttu-id="30e52-128">String</span><span class="sxs-lookup"><span data-stu-id="30e52-128">String</span></span>     |<span data-ttu-id="30e52-129">ディレクトリの名前です。</span><span class="sxs-lookup"><span data-stu-id="30e52-129">Name of the directory.</span></span> <span data-ttu-id="30e52-130">[同期スキーマ](synchronization-synchronizationschema.md)内で一意である必要があります。</span><span class="sxs-lookup"><span data-stu-id="30e52-130">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="30e52-131">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="30e52-131">Not nullable.</span></span>|
|<span data-ttu-id="30e52-132">オブジェクト</span><span class="sxs-lookup"><span data-stu-id="30e52-132">objects</span></span>        |<span data-ttu-id="30e52-133">[objectDefinition](synchronization-objectdefinition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="30e52-133">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="30e52-134">ディレクトリでサポートされているオブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="30e52-134">Collection of objects supported by the directory.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="30e52-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="30e52-135">JSON representation</span></span>

<span data-ttu-id="30e52-136">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="30e52-136">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-example"></a><span data-ttu-id="30e52-137">JSON の例</span><span class="sxs-lookup"><span data-stu-id="30e52-137">JSON Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "directoryDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->