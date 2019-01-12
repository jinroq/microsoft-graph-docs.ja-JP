---
title: emailAddress リソースの種類
description: 名前およびエンティティのインスタンスの SMTP アドレスを表すなど、メッセージの受信者、または予定表の所有者です。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: c06849a73f4246653b8d78dcd392c4e4f6686a46
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932792"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="01dc5-103">emailAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="01dc5-103">emailAddress resource type</span></span>

> <span data-ttu-id="01dc5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="01dc5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01dc5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="01dc5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01dc5-106">名前およびエンティティのインスタンスの SMTP アドレスを表すなど、メッセージの受信者、または予定表の所有者です。</span><span class="sxs-lookup"><span data-stu-id="01dc5-106">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="01dc5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="01dc5-107">Properties</span></span>
| <span data-ttu-id="01dc5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="01dc5-108">Property</span></span>     | <span data-ttu-id="01dc5-109">種類</span><span class="sxs-lookup"><span data-stu-id="01dc5-109">Type</span></span>   |<span data-ttu-id="01dc5-110">説明</span><span class="sxs-lookup"><span data-stu-id="01dc5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01dc5-111">address</span><span class="sxs-lookup"><span data-stu-id="01dc5-111">address</span></span>|<span data-ttu-id="01dc5-112">String</span><span class="sxs-lookup"><span data-stu-id="01dc5-112">String</span></span>|<span data-ttu-id="01dc5-113">エンティティ インスタンスの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="01dc5-113">The email address of an entity instance.</span></span>|
|<span data-ttu-id="01dc5-114">名前</span><span class="sxs-lookup"><span data-stu-id="01dc5-114">name</span></span>|<span data-ttu-id="01dc5-115">String</span><span class="sxs-lookup"><span data-stu-id="01dc5-115">String</span></span>|<span data-ttu-id="01dc5-116">エンティティ インスタンスの表示名。</span><span class="sxs-lookup"><span data-stu-id="01dc5-116">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="01dc5-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="01dc5-117">JSON representation</span></span>

<span data-ttu-id="01dc5-118">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="01dc5-118">Here is a JSON representation of the resource</span></span>

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
