---
title: onPremisesProvisioningError リソースの種類
description: 同期、オンプレミス Azure Active Directory へのディレクトリは、ユーザー、グループ、または組織の取引先担当者エンティティのディレクトリ同期のエラーを表します。
localization_priority: Normal
ms.openlocfilehash: 1ea9efcd4d9db5cf7cc5b8f0a18b35345d06c3fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817739"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="015fa-103">onPremisesProvisioningError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="015fa-103">onPremisesProvisioningError resource type</span></span>

> <span data-ttu-id="015fa-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="015fa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="015fa-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="015fa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="015fa-106">同期、オンプレミス Azure Active Directory へのディレクトリは、[ユーザー](user.md)、[グループ](group.md)、または[組織の連絡先](orgcontact.md)のエンティティのディレクトリ同期のエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="015fa-106">Represents directory synchronization errors for the [user](user.md), [group](group.md), or [organizational contact](orgcontact.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="015fa-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="015fa-107">Properties</span></span>

| <span data-ttu-id="015fa-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="015fa-108">Property</span></span> | <span data-ttu-id="015fa-109">種類</span><span class="sxs-lookup"><span data-stu-id="015fa-109">Type</span></span> | <span data-ttu-id="015fa-110">説明</span><span class="sxs-lookup"><span data-stu-id="015fa-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="015fa-111">category</span><span class="sxs-lookup"><span data-stu-id="015fa-111">category</span></span>|<span data-ttu-id="015fa-112">String</span><span class="sxs-lookup"><span data-stu-id="015fa-112">String</span></span>| <span data-ttu-id="015fa-113">プロビジョニングのエラーのカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="015fa-113">Category of the provisioning error.</span></span> <span data-ttu-id="015fa-114">注意: 現時点が 1 つだけ使用可能な値です。</span><span class="sxs-lookup"><span data-stu-id="015fa-114">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="015fa-115">使用可能な値: *PropertyConflict* - は、プロパティの値が一意でないことを示します。</span><span class="sxs-lookup"><span data-stu-id="015fa-115">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="015fa-116">その他のオブジェクトには、プロパティに対して同じ値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="015fa-116">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="015fa-117">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="015fa-117">occurredDateTime</span></span>|<span data-ttu-id="015fa-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="015fa-118">DateTimeOffset</span></span>| <span data-ttu-id="015fa-119">日付と時刻、エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="015fa-119">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="015fa-120">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="015fa-120">propertyCausingError</span></span>|<span data-ttu-id="015fa-121">String</span><span class="sxs-lookup"><span data-stu-id="015fa-121">String</span></span>| <span data-ttu-id="015fa-122">エラーの原因でディレクトリのプロパティの名前です。</span><span class="sxs-lookup"><span data-stu-id="015fa-122">Name of the directory property causing the error.</span></span> <span data-ttu-id="015fa-123">現在使用可能な値: *UserPrincipalName*または*メタベース*</span><span class="sxs-lookup"><span data-stu-id="015fa-123">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="015fa-124">value</span><span class="sxs-lookup"><span data-stu-id="015fa-124">value</span></span>|<span data-ttu-id="015fa-125">文字列</span><span class="sxs-lookup"><span data-stu-id="015fa-125">String</span></span>| <span data-ttu-id="015fa-126">エラーの原因で、プロパティの値です。</span><span class="sxs-lookup"><span data-stu-id="015fa-126">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="015fa-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="015fa-127">JSON representation</span></span>
<span data-ttu-id="015fa-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="015fa-128">Here is a JSON representation of the resource.</span></span>

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
