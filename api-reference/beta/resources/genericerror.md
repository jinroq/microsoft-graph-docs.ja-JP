---
title: genericError リソースの種類
description: 汎用のエラーです。
ms.openlocfilehash: caf3fbb99ad521fd807138ab230f6a1b8ae7bb16
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067166"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="8d0a5-103">genericError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8d0a5-103">genericError resource type</span></span>

> <span data-ttu-id="8d0a5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8d0a5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d0a5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d0a5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8d0a5-106">汎用のエラーです。</span><span class="sxs-lookup"><span data-stu-id="8d0a5-106">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="8d0a5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d0a5-107">Properties</span></span>

| <span data-ttu-id="8d0a5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d0a5-108">Property</span></span> | <span data-ttu-id="8d0a5-109">型</span><span class="sxs-lookup"><span data-stu-id="8d0a5-109">Type</span></span> | <span data-ttu-id="8d0a5-110">説明</span><span class="sxs-lookup"><span data-stu-id="8d0a5-110">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="8d0a5-111">message</span><span class="sxs-lookup"><span data-stu-id="8d0a5-111">message</span></span> | <span data-ttu-id="8d0a5-112">String</span><span class="sxs-lookup"><span data-stu-id="8d0a5-112">String</span></span> | <span data-ttu-id="8d0a5-113">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="8d0a5-113">The error message.</span></span> |
| <span data-ttu-id="8d0a5-114">code</span><span class="sxs-lookup"><span data-stu-id="8d0a5-114">code</span></span> | <span data-ttu-id="8d0a5-115">String</span><span class="sxs-lookup"><span data-stu-id="8d0a5-115">String</span></span> | <span data-ttu-id="8d0a5-116">エラー コード。</span><span class="sxs-lookup"><span data-stu-id="8d0a5-116">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8d0a5-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8d0a5-117">JSON representation</span></span>

<span data-ttu-id="8d0a5-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8d0a5-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.genericError"
}-->

```json
{
  "message": "String",
  "code": "String"
}
```