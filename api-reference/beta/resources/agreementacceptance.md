---
title: agreementAcceptance リソースの種類
description: azure Active Directory (azure AD) によって提供される会社のカスタマイズ可能な使用条件の範囲内でのユーザーの現在の状態を表します。
localization_priority: Normal
ms.openlocfilehash: 884a6b7dcf4dcc8f00aa927dd9d486c074b64183
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544063"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="b1fe8-103">agreementAcceptance リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b1fe8-103">agreementAcceptance resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1fe8-104">azure Active Directory (azure AD) によって提供される会社のカスタマイズ可能な使用条件の範囲内でのユーザーの現在の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="b1fe8-104">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a><span data-ttu-id="b1fe8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1fe8-105">Properties</span></span>
| <span data-ttu-id="b1fe8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1fe8-106">Property</span></span>     | <span data-ttu-id="b1fe8-107">型</span><span class="sxs-lookup"><span data-stu-id="b1fe8-107">Type</span></span>        | <span data-ttu-id="b1fe8-108">説明</span><span class="sxs-lookup"><span data-stu-id="b1fe8-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b1fe8-109">agreementFileId</span><span class="sxs-lookup"><span data-stu-id="b1fe8-109">agreementFileId</span></span>|<span data-ttu-id="b1fe8-110">String</span><span class="sxs-lookup"><span data-stu-id="b1fe8-110">String</span></span>|<span data-ttu-id="b1fe8-111">ユーザーによって承認されたアグリーメントファイルの ID。</span><span class="sxs-lookup"><span data-stu-id="b1fe8-111">ID of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="b1fe8-112">agreementId</span><span class="sxs-lookup"><span data-stu-id="b1fe8-112">agreementId</span></span>|<span data-ttu-id="b1fe8-113">String</span><span class="sxs-lookup"><span data-stu-id="b1fe8-113">String</span></span>|<span data-ttu-id="b1fe8-114">契約の ID。</span><span class="sxs-lookup"><span data-stu-id="b1fe8-114">ID of the agreement.</span></span>|
|<span data-ttu-id="b1fe8-115">id</span><span class="sxs-lookup"><span data-stu-id="b1fe8-115">id</span></span>|<span data-ttu-id="b1fe8-116">String</span><span class="sxs-lookup"><span data-stu-id="b1fe8-116">String</span></span>| <span data-ttu-id="b1fe8-117">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b1fe8-117">Read-only.</span></span>|
|<span data-ttu-id="b1fe8-118">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1fe8-118">recordedDateTime</span></span>|<span data-ttu-id="b1fe8-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1fe8-119">DateTimeOffset</span></span>|<span data-ttu-id="b1fe8-p101">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b1fe8-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b1fe8-122">state</span><span class="sxs-lookup"><span data-stu-id="b1fe8-122">state</span></span>|<span data-ttu-id="b1fe8-123">string</span><span class="sxs-lookup"><span data-stu-id="b1fe8-123">string</span></span>| <span data-ttu-id="b1fe8-124">可能な値は、`accepted`、`declined` です。</span><span class="sxs-lookup"><span data-stu-id="b1fe8-124">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="b1fe8-125">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="b1fe8-125">userDisplayName</span></span>|<span data-ttu-id="b1fe8-126">String</span><span class="sxs-lookup"><span data-stu-id="b1fe8-126">String</span></span>|<span data-ttu-id="b1fe8-127">承諾が記録されたときのユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="b1fe8-127">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="b1fe8-128">userEmail</span><span class="sxs-lookup"><span data-stu-id="b1fe8-128">userEmail</span></span>|<span data-ttu-id="b1fe8-129">String</span><span class="sxs-lookup"><span data-stu-id="b1fe8-129">String</span></span>|<span data-ttu-id="b1fe8-130">承諾が記録されたユーザーの電子メール。</span><span class="sxs-lookup"><span data-stu-id="b1fe8-130">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="b1fe8-131">userId</span><span class="sxs-lookup"><span data-stu-id="b1fe8-131">userId</span></span>|<span data-ttu-id="b1fe8-132">String</span><span class="sxs-lookup"><span data-stu-id="b1fe8-132">String</span></span>|<span data-ttu-id="b1fe8-133">契約書を受諾したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="b1fe8-133">ID of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="b1fe8-134">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b1fe8-134">userPrincipalName</span></span>|<span data-ttu-id="b1fe8-135">String</span><span class="sxs-lookup"><span data-stu-id="b1fe8-135">String</span></span>|<span data-ttu-id="b1fe8-136">承諾が記録されたユーザーの UPN。</span><span class="sxs-lookup"><span data-stu-id="b1fe8-136">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1fe8-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b1fe8-137">Relationships</span></span>
<span data-ttu-id="b1fe8-138">なし</span><span class="sxs-lookup"><span data-stu-id="b1fe8-138">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b1fe8-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b1fe8-139">JSON representation</span></span>

<span data-ttu-id="b1fe8-140">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b1fe8-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementAcceptance"
}-->

```json
{
  "agreementFileId": "String",
  "agreementId": "String",
  "id": "String (identifier)",
  "recordedDateTime": "String (timestamp)",
  "state": "string",
  "userDisplayName": "String",
  "userEmail": "String",
  "userId": "String",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementAcceptance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/agreementacceptance.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
