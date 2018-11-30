---
title: onPremisesProvisioningError リソースの種類
description: Azure Active Directory への設置型のディレクトリを同期するときは、ユーザーとグループのエンティティのディレクトリ同期のエラーを表します。
ms.openlocfilehash: 7d5b15d99559ddf5b7692b7eac9664de7ec50f1e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024193"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="c0609-103">onPremisesProvisioningError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c0609-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="c0609-104">同期、オンプレミス Azure Active Directory へのディレクトリは、[ユーザー](user.md)と[グループ](group.md)のエンティティのディレクトリ同期のエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="c0609-104">Represents directory synchronization errors for the [user](user.md) and [group](group.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="c0609-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0609-105">Properties</span></span>

| <span data-ttu-id="c0609-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0609-106">Property</span></span> | <span data-ttu-id="c0609-107">型</span><span class="sxs-lookup"><span data-stu-id="c0609-107">Type</span></span> | <span data-ttu-id="c0609-108">説明</span><span class="sxs-lookup"><span data-stu-id="c0609-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c0609-109">category</span><span class="sxs-lookup"><span data-stu-id="c0609-109">category</span></span>|<span data-ttu-id="c0609-110">String</span><span class="sxs-lookup"><span data-stu-id="c0609-110">String</span></span>| <span data-ttu-id="c0609-111">プロビジョニングのエラーのカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="c0609-111">Category of the provisioning error.</span></span> <span data-ttu-id="c0609-112">注意: 現時点が 1 つだけ使用可能な値です。</span><span class="sxs-lookup"><span data-stu-id="c0609-112">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="c0609-113">使用可能な値: *PropertyConflict* - は、プロパティの値が一意でないことを示します。</span><span class="sxs-lookup"><span data-stu-id="c0609-113">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="c0609-114">その他のオブジェクトには、プロパティに対して同じ値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c0609-114">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="c0609-115">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="c0609-115">occurredDateTime</span></span>|<span data-ttu-id="c0609-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0609-116">DateTimeOffset</span></span>| <span data-ttu-id="c0609-117">日付と時刻、エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="c0609-117">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="c0609-118">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="c0609-118">propertyCausingError</span></span>|<span data-ttu-id="c0609-119">String</span><span class="sxs-lookup"><span data-stu-id="c0609-119">String</span></span>| <span data-ttu-id="c0609-120">エラーの原因でディレクトリのプロパティの名前です。</span><span class="sxs-lookup"><span data-stu-id="c0609-120">Name of the directory property causing the error.</span></span> <span data-ttu-id="c0609-121">現在使用可能な値: *UserPrincipalName*または*メタベース*</span><span class="sxs-lookup"><span data-stu-id="c0609-121">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="c0609-122">value</span><span class="sxs-lookup"><span data-stu-id="c0609-122">value</span></span>|<span data-ttu-id="c0609-123">文字列</span><span class="sxs-lookup"><span data-stu-id="c0609-123">String</span></span>| <span data-ttu-id="c0609-124">エラーの原因で、プロパティの値です。</span><span class="sxs-lookup"><span data-stu-id="c0609-124">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c0609-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c0609-125">JSON representation</span></span>
<span data-ttu-id="c0609-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c0609-126">Here is a JSON representation of the resource.</span></span>

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