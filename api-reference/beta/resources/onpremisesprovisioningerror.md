---
title: onPremisesProvisioningError リソースの種類
description: オンプレミスのディレクトリを Azure Active directory と同期するときの、ユーザー、グループ、または組織の連絡先エンティティのディレクトリ同期エラーを表します。
localization_priority: Normal
ms.openlocfilehash: 7e4d51ea3bde6158256c607027b3e56236a8151c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568851"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="c6dfa-103">onPremisesProvisioningError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c6dfa-103">onPremisesProvisioningError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6dfa-104">オンプレミスのディレクトリを Azure Active directory と同期するときの、[ユーザー](user.md)、[グループ](group.md)、または[組織の連絡先](orgcontact.md)エンティティのディレクトリ同期エラーを表します。</span><span class="sxs-lookup"><span data-stu-id="c6dfa-104">Represents directory synchronization errors for the [user](user.md), [group](group.md), or [organizational contact](orgcontact.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="c6dfa-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6dfa-105">Properties</span></span>

| <span data-ttu-id="c6dfa-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6dfa-106">Property</span></span> | <span data-ttu-id="c6dfa-107">型</span><span class="sxs-lookup"><span data-stu-id="c6dfa-107">Type</span></span> | <span data-ttu-id="c6dfa-108">説明</span><span class="sxs-lookup"><span data-stu-id="c6dfa-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c6dfa-109">category</span><span class="sxs-lookup"><span data-stu-id="c6dfa-109">category</span></span>|<span data-ttu-id="c6dfa-110">String</span><span class="sxs-lookup"><span data-stu-id="c6dfa-110">String</span></span>| <span data-ttu-id="c6dfa-111">プロビジョニングエラーのカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="c6dfa-111">Category of the provisioning error.</span></span> <span data-ttu-id="c6dfa-112">注: 現時点では、可能な値は1つだけです。</span><span class="sxs-lookup"><span data-stu-id="c6dfa-112">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="c6dfa-113">可能な値: *propertyconflict* -プロパティ値が一意ではないことを示します。</span><span class="sxs-lookup"><span data-stu-id="c6dfa-113">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="c6dfa-114">その他のオブジェクトには、プロパティと同じ値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c6dfa-114">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="c6dfa-115">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="c6dfa-115">occurredDateTime</span></span>|<span data-ttu-id="c6dfa-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6dfa-116">DateTimeOffset</span></span>| <span data-ttu-id="c6dfa-117">エラーが発生した日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="c6dfa-117">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="c6dfa-118">propertycain error</span><span class="sxs-lookup"><span data-stu-id="c6dfa-118">propertyCausingError</span></span>|<span data-ttu-id="c6dfa-119">String</span><span class="sxs-lookup"><span data-stu-id="c6dfa-119">String</span></span>| <span data-ttu-id="c6dfa-120">エラーを引き起こしたディレクトリプロパティの名前。</span><span class="sxs-lookup"><span data-stu-id="c6dfa-120">Name of the directory property causing the error.</span></span> <span data-ttu-id="c6dfa-121">現在使用可能な値: *UserPrincipalName*または*ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="c6dfa-121">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="c6dfa-122">value</span><span class="sxs-lookup"><span data-stu-id="c6dfa-122">value</span></span>|<span data-ttu-id="c6dfa-123">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c6dfa-123">String</span></span>| <span data-ttu-id="c6dfa-124">エラーが発生したプロパティの値。</span><span class="sxs-lookup"><span data-stu-id="c6dfa-124">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c6dfa-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c6dfa-125">JSON representation</span></span>
<span data-ttu-id="c6dfa-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c6dfa-126">Here is a JSON representation of the resource.</span></span>

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
