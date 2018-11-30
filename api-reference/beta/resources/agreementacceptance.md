---
title: agreementAcceptance リソースの種類
description: Azure Active Directory (Azure AD) の電源を使用して会社のカスタマイズ可能な条件の範囲内のユーザーの現在の状態を表します。
ms.openlocfilehash: 23221fe88a65b003c8d26aca99eaf1f03d935722
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066479"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="74ad5-103">agreementAcceptance リソースの種類</span><span class="sxs-lookup"><span data-stu-id="74ad5-103">agreementAcceptance resource type</span></span>

> <span data-ttu-id="74ad5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="74ad5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74ad5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74ad5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="74ad5-106">Azure Active Directory (Azure AD) の電源を使用して会社のカスタマイズ可能な条件の範囲内のユーザーの現在の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="74ad5-106">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a><span data-ttu-id="74ad5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74ad5-107">Properties</span></span>
| <span data-ttu-id="74ad5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74ad5-108">Property</span></span>     | <span data-ttu-id="74ad5-109">型</span><span class="sxs-lookup"><span data-stu-id="74ad5-109">Type</span></span>        | <span data-ttu-id="74ad5-110">説明</span><span class="sxs-lookup"><span data-stu-id="74ad5-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="74ad5-111">agreementFileId</span><span class="sxs-lookup"><span data-stu-id="74ad5-111">agreementFileId</span></span>|<span data-ttu-id="74ad5-112">String</span><span class="sxs-lookup"><span data-stu-id="74ad5-112">String</span></span>|<span data-ttu-id="74ad5-113">ユーザーによって承諾される契約書のファイルの ID です。</span><span class="sxs-lookup"><span data-stu-id="74ad5-113">ID of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="74ad5-114">agreementId</span><span class="sxs-lookup"><span data-stu-id="74ad5-114">agreementId</span></span>|<span data-ttu-id="74ad5-115">String</span><span class="sxs-lookup"><span data-stu-id="74ad5-115">String</span></span>|<span data-ttu-id="74ad5-116">契約の ID です。</span><span class="sxs-lookup"><span data-stu-id="74ad5-116">ID of the agreement.</span></span>|
|<span data-ttu-id="74ad5-117">id</span><span class="sxs-lookup"><span data-stu-id="74ad5-117">id</span></span>|<span data-ttu-id="74ad5-118">String</span><span class="sxs-lookup"><span data-stu-id="74ad5-118">String</span></span>| <span data-ttu-id="74ad5-119">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="74ad5-119">Read-only.</span></span>|
|<span data-ttu-id="74ad5-120">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="74ad5-120">recordedDateTime</span></span>|<span data-ttu-id="74ad5-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74ad5-121">DateTimeOffset</span></span>|<span data-ttu-id="74ad5-p102">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="74ad5-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="74ad5-124">state</span><span class="sxs-lookup"><span data-stu-id="74ad5-124">state</span></span>|<span data-ttu-id="74ad5-125">文字列</span><span class="sxs-lookup"><span data-stu-id="74ad5-125">string</span></span>| <span data-ttu-id="74ad5-126">使用可能な値は、`accepted`、`declined` です。</span><span class="sxs-lookup"><span data-stu-id="74ad5-126">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="74ad5-127">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="74ad5-127">userDisplayName</span></span>|<span data-ttu-id="74ad5-128">String</span><span class="sxs-lookup"><span data-stu-id="74ad5-128">String</span></span>|<span data-ttu-id="74ad5-129">受け入れの記録時に、ユーザーの名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="74ad5-129">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="74ad5-130">userEmail</span><span class="sxs-lookup"><span data-stu-id="74ad5-130">userEmail</span></span>|<span data-ttu-id="74ad5-131">String</span><span class="sxs-lookup"><span data-stu-id="74ad5-131">String</span></span>|<span data-ttu-id="74ad5-132">受け入れが記録された場合のユーザーの電子メール。</span><span class="sxs-lookup"><span data-stu-id="74ad5-132">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="74ad5-133">userId</span><span class="sxs-lookup"><span data-stu-id="74ad5-133">userId</span></span>|<span data-ttu-id="74ad5-134">String</span><span class="sxs-lookup"><span data-stu-id="74ad5-134">String</span></span>|<span data-ttu-id="74ad5-135">契約を承諾したユーザーの ID です。</span><span class="sxs-lookup"><span data-stu-id="74ad5-135">ID of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="74ad5-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="74ad5-136">userPrincipalName</span></span>|<span data-ttu-id="74ad5-137">String</span><span class="sxs-lookup"><span data-stu-id="74ad5-137">String</span></span>|<span data-ttu-id="74ad5-138">受け入れが記録された場合のユーザーの UPN。</span><span class="sxs-lookup"><span data-stu-id="74ad5-138">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74ad5-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="74ad5-139">Relationships</span></span>
<span data-ttu-id="74ad5-140">なし</span><span class="sxs-lookup"><span data-stu-id="74ad5-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="74ad5-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="74ad5-141">JSON representation</span></span>

<span data-ttu-id="74ad5-142">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74ad5-142">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "agreementAcceptance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
