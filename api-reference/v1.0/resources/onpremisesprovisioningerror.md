---
title: onPremisesProvisioningError リソースの種類
description: オンプレミスのディレクトリを Azure Active Directory と同期するときに、ユーザーエンティティおよびグループエンティティのディレクトリ同期エラーを表します。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3fd16b43d35cb12e7b9c7f82dc59f940994bc1b1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035749"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="1d125-103">onPremisesProvisioningError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1d125-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="1d125-104">オンプレミスのディレクトリを Azure Active Directory と同期するときに、[ユーザー](user.md)エンティティおよび[グループ](group.md)エンティティのディレクトリ同期エラーを表します。</span><span class="sxs-lookup"><span data-stu-id="1d125-104">Represents directory synchronization errors for the [user](user.md) and [group](group.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="1d125-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d125-105">Properties</span></span>

| <span data-ttu-id="1d125-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d125-106">Property</span></span> | <span data-ttu-id="1d125-107">型</span><span class="sxs-lookup"><span data-stu-id="1d125-107">Type</span></span> | <span data-ttu-id="1d125-108">説明</span><span class="sxs-lookup"><span data-stu-id="1d125-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1d125-109">category</span><span class="sxs-lookup"><span data-stu-id="1d125-109">category</span></span>|<span data-ttu-id="1d125-110">String</span><span class="sxs-lookup"><span data-stu-id="1d125-110">String</span></span>| <span data-ttu-id="1d125-111">プロビジョニングエラーのカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="1d125-111">Category of the provisioning error.</span></span> <span data-ttu-id="1d125-112">注: 現時点では、可能な値は1つだけです。</span><span class="sxs-lookup"><span data-stu-id="1d125-112">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="1d125-113">可能な値: *Propertyconflict* -プロパティ値が一意ではないことを示します。</span><span class="sxs-lookup"><span data-stu-id="1d125-113">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="1d125-114">その他のオブジェクトには、プロパティと同じ値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1d125-114">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="1d125-115">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="1d125-115">occurredDateTime</span></span>|<span data-ttu-id="1d125-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d125-116">DateTimeOffset</span></span>| <span data-ttu-id="1d125-117">エラーが発生した日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="1d125-117">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="1d125-118">Propertycain Error</span><span class="sxs-lookup"><span data-stu-id="1d125-118">propertyCausingError</span></span>|<span data-ttu-id="1d125-119">String</span><span class="sxs-lookup"><span data-stu-id="1d125-119">String</span></span>| <span data-ttu-id="1d125-120">エラーを引き起こしたディレクトリプロパティの名前。</span><span class="sxs-lookup"><span data-stu-id="1d125-120">Name of the directory property causing the error.</span></span> <span data-ttu-id="1d125-121">現在使用可能な値: *UserPrincipalName*または*ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="1d125-121">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="1d125-122">value</span><span class="sxs-lookup"><span data-stu-id="1d125-122">value</span></span>|<span data-ttu-id="1d125-123">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1d125-123">String</span></span>| <span data-ttu-id="1d125-124">エラーが発生したプロパティの値。</span><span class="sxs-lookup"><span data-stu-id="1d125-124">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1d125-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1d125-125">JSON representation</span></span>
<span data-ttu-id="1d125-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1d125-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
