---
title: chatMessageMention リソースの種類
description: 'ChatMessage エンティティの参照を表します。 ユーザー、チーム、ボットまたはチャネルをことができます。 '
localization_priority: Normal
ms.openlocfilehash: 7b24d2af6f61f3da69480557e1c5b5f32c009c25
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876140"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="d6b1a-104">chatMessageMention リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d6b1a-104">chatMessageMention resource type</span></span>

> <span data-ttu-id="d6b1a-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d6b1a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6b1a-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6b1a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d6b1a-107">[ChatMessage](chatmessage.md)エンティティの参照を表します。</span><span class="sxs-lookup"><span data-stu-id="d6b1a-107">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="d6b1a-108">ユーザー、チーム、ボットまたはチャネルをことができます。</span><span class="sxs-lookup"><span data-stu-id="d6b1a-108">The mention can be to a user, team, bot or channel.</span></span> 

## <a name="properties"></a><span data-ttu-id="d6b1a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6b1a-109">Properties</span></span>
| <span data-ttu-id="d6b1a-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6b1a-110">Property</span></span>     | <span data-ttu-id="d6b1a-111">種類</span><span class="sxs-lookup"><span data-stu-id="d6b1a-111">Type</span></span>   |<span data-ttu-id="d6b1a-112">説明</span><span class="sxs-lookup"><span data-stu-id="d6b1a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6b1a-113">ID</span><span class="sxs-lookup"><span data-stu-id="d6b1a-113">id</span></span>|<span data-ttu-id="d6b1a-114">文字列</span><span class="sxs-lookup"><span data-stu-id="d6b1a-114">string</span></span>|<span data-ttu-id="d6b1a-115">記載されているエンティティの id</span><span class="sxs-lookup"><span data-stu-id="d6b1a-115">Id of the entity being mentioned</span></span>|
|<span data-ttu-id="d6b1a-116">mentionText</span><span class="sxs-lookup"><span data-stu-id="d6b1a-116">mentionText</span></span>|<span data-ttu-id="d6b1a-117">文字列</span><span class="sxs-lookup"><span data-stu-id="d6b1a-117">string</span></span>|<span data-ttu-id="d6b1a-118">Ex の説明を表すために使用する文字列: ユーザーの表示名、チーム名等</span><span class="sxs-lookup"><span data-stu-id="d6b1a-118">String used to represent the mention Ex: User display name, Team name etc</span></span>|
|<span data-ttu-id="d6b1a-119">記載されています。</span><span class="sxs-lookup"><span data-stu-id="d6b1a-119">mentioned</span></span>|[<span data-ttu-id="d6b1a-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="d6b1a-120">identitySet</span></span>](identityset.md)|<span data-ttu-id="d6b1a-121">記載されているユーザー</span><span class="sxs-lookup"><span data-stu-id="d6b1a-121">The user that was mentioned</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d6b1a-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d6b1a-122">JSON representation</span></span>

<span data-ttu-id="d6b1a-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d6b1a-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": "string (identifier)",
  "mentionText": "string",
  "mentioned": "microsoft.graph.identitySet"
 }

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
