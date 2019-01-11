---
title: emailAddress リソースの種類
description: 名前およびエンティティのインスタンスの SMTP アドレスを表すなど、メッセージの受信者、または予定表の所有者です。
localization_priority: Normal
ms.openlocfilehash: 5286334378aa5d208cf171ecab0bdc1777a4073b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871226"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="13d6b-103">emailAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="13d6b-103">emailAddress resource type</span></span>

> <span data-ttu-id="13d6b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="13d6b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13d6b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13d6b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13d6b-106">名前およびエンティティのインスタンスの SMTP アドレスを表すなど、メッセージの受信者、または予定表の所有者です。</span><span class="sxs-lookup"><span data-stu-id="13d6b-106">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="13d6b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13d6b-107">Properties</span></span>
| <span data-ttu-id="13d6b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13d6b-108">Property</span></span>     | <span data-ttu-id="13d6b-109">種類</span><span class="sxs-lookup"><span data-stu-id="13d6b-109">Type</span></span>   |<span data-ttu-id="13d6b-110">説明</span><span class="sxs-lookup"><span data-stu-id="13d6b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13d6b-111">address</span><span class="sxs-lookup"><span data-stu-id="13d6b-111">address</span></span>|<span data-ttu-id="13d6b-112">String</span><span class="sxs-lookup"><span data-stu-id="13d6b-112">String</span></span>|<span data-ttu-id="13d6b-113">エンティティ インスタンスの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="13d6b-113">The email address of an entity instance.</span></span>|
|<span data-ttu-id="13d6b-114">名前</span><span class="sxs-lookup"><span data-stu-id="13d6b-114">name</span></span>|<span data-ttu-id="13d6b-115">String</span><span class="sxs-lookup"><span data-stu-id="13d6b-115">String</span></span>|<span data-ttu-id="13d6b-116">エンティティ インスタンスの表示名。</span><span class="sxs-lookup"><span data-stu-id="13d6b-116">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13d6b-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="13d6b-117">JSON representation</span></span>

<span data-ttu-id="13d6b-118">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="13d6b-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailAddress"
}-->

```json
{
  "address": "string",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
