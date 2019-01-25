---
title: onPremisesProvisioningError リソースの種類
description: 同期、オンプレミス Azure Active Directory へのディレクトリは、ユーザー、グループ、または組織の取引先担当者エンティティのディレクトリ同期のエラーを表します。
localization_priority: Normal
ms.openlocfilehash: 7e4d51ea3bde6158256c607027b3e56236a8151c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512732"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="eafbb-103">onPremisesProvisioningError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eafbb-103">onPremisesProvisioningError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eafbb-104">同期、オンプレミス Azure Active Directory へのディレクトリは、[ユーザー](user.md)、[グループ](group.md)、または[組織の連絡先](orgcontact.md)のエンティティのディレクトリ同期のエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="eafbb-104">Represents directory synchronization errors for the [user](user.md), [group](group.md), or [organizational contact](orgcontact.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="eafbb-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eafbb-105">Properties</span></span>

| <span data-ttu-id="eafbb-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eafbb-106">Property</span></span> | <span data-ttu-id="eafbb-107">型</span><span class="sxs-lookup"><span data-stu-id="eafbb-107">Type</span></span> | <span data-ttu-id="eafbb-108">説明</span><span class="sxs-lookup"><span data-stu-id="eafbb-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="eafbb-109">category</span><span class="sxs-lookup"><span data-stu-id="eafbb-109">category</span></span>|<span data-ttu-id="eafbb-110">String</span><span class="sxs-lookup"><span data-stu-id="eafbb-110">String</span></span>| <span data-ttu-id="eafbb-111">プロビジョニングのエラーのカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="eafbb-111">Category of the provisioning error.</span></span> <span data-ttu-id="eafbb-112">注意: 現時点が 1 つだけ使用可能な値です。</span><span class="sxs-lookup"><span data-stu-id="eafbb-112">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="eafbb-113">使用可能な値: *PropertyConflict* - は、プロパティの値が一意でないことを示します。</span><span class="sxs-lookup"><span data-stu-id="eafbb-113">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="eafbb-114">その他のオブジェクトには、プロパティに対して同じ値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="eafbb-114">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="eafbb-115">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="eafbb-115">occurredDateTime</span></span>|<span data-ttu-id="eafbb-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eafbb-116">DateTimeOffset</span></span>| <span data-ttu-id="eafbb-117">日付と時刻、エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="eafbb-117">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="eafbb-118">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="eafbb-118">propertyCausingError</span></span>|<span data-ttu-id="eafbb-119">String</span><span class="sxs-lookup"><span data-stu-id="eafbb-119">String</span></span>| <span data-ttu-id="eafbb-120">エラーの原因でディレクトリのプロパティの名前です。</span><span class="sxs-lookup"><span data-stu-id="eafbb-120">Name of the directory property causing the error.</span></span> <span data-ttu-id="eafbb-121">現在使用可能な値: *UserPrincipalName*または*メタベース*</span><span class="sxs-lookup"><span data-stu-id="eafbb-121">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="eafbb-122">value</span><span class="sxs-lookup"><span data-stu-id="eafbb-122">value</span></span>|<span data-ttu-id="eafbb-123">文字列</span><span class="sxs-lookup"><span data-stu-id="eafbb-123">String</span></span>| <span data-ttu-id="eafbb-124">エラーの原因で、プロパティの値です。</span><span class="sxs-lookup"><span data-stu-id="eafbb-124">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eafbb-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eafbb-125">JSON representation</span></span>
<span data-ttu-id="eafbb-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eafbb-126">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisesprovisioningerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
