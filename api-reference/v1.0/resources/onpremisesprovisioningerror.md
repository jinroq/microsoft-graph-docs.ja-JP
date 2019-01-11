---
title: onPremisesProvisioningError リソースの種類
description: Azure Active Directory への設置型のディレクトリを同期するときは、ユーザーとグループのエンティティのディレクトリ同期のエラーを表します。
localization_priority: Normal
ms.openlocfilehash: c8989a78dfb60a6c7c25a66a9f1e619dcbdca15d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830668"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="84b31-103">onPremisesProvisioningError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="84b31-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="84b31-104">同期、オンプレミス Azure Active Directory へのディレクトリは、[ユーザー](user.md)と[グループ](group.md)のエンティティのディレクトリ同期のエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="84b31-104">Represents directory synchronization errors for the [user](user.md) and [group](group.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="84b31-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84b31-105">Properties</span></span>

| <span data-ttu-id="84b31-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84b31-106">Property</span></span> | <span data-ttu-id="84b31-107">種類</span><span class="sxs-lookup"><span data-stu-id="84b31-107">Type</span></span> | <span data-ttu-id="84b31-108">説明</span><span class="sxs-lookup"><span data-stu-id="84b31-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="84b31-109">category</span><span class="sxs-lookup"><span data-stu-id="84b31-109">category</span></span>|<span data-ttu-id="84b31-110">String</span><span class="sxs-lookup"><span data-stu-id="84b31-110">String</span></span>| <span data-ttu-id="84b31-111">プロビジョニングのエラーのカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="84b31-111">Category of the provisioning error.</span></span> <span data-ttu-id="84b31-112">注意: 現時点が 1 つだけ使用可能な値です。</span><span class="sxs-lookup"><span data-stu-id="84b31-112">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="84b31-113">使用可能な値: *PropertyConflict* - は、プロパティの値が一意でないことを示します。</span><span class="sxs-lookup"><span data-stu-id="84b31-113">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="84b31-114">その他のオブジェクトには、プロパティに対して同じ値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="84b31-114">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="84b31-115">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="84b31-115">occurredDateTime</span></span>|<span data-ttu-id="84b31-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84b31-116">DateTimeOffset</span></span>| <span data-ttu-id="84b31-117">日付と時刻、エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="84b31-117">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="84b31-118">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="84b31-118">propertyCausingError</span></span>|<span data-ttu-id="84b31-119">String</span><span class="sxs-lookup"><span data-stu-id="84b31-119">String</span></span>| <span data-ttu-id="84b31-120">エラーの原因でディレクトリのプロパティの名前です。</span><span class="sxs-lookup"><span data-stu-id="84b31-120">Name of the directory property causing the error.</span></span> <span data-ttu-id="84b31-121">現在使用可能な値: *UserPrincipalName*または*メタベース*</span><span class="sxs-lookup"><span data-stu-id="84b31-121">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="84b31-122">value</span><span class="sxs-lookup"><span data-stu-id="84b31-122">value</span></span>|<span data-ttu-id="84b31-123">文字列</span><span class="sxs-lookup"><span data-stu-id="84b31-123">String</span></span>| <span data-ttu-id="84b31-124">エラーの原因で、プロパティの値です。</span><span class="sxs-lookup"><span data-stu-id="84b31-124">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="84b31-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="84b31-125">JSON representation</span></span>
<span data-ttu-id="84b31-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="84b31-126">Here is a JSON representation of the resource.</span></span>

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
