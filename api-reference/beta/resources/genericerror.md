---
title: genericError リソースの種類
description: 汎用のエラーです。
localization_priority: Normal
ms.openlocfilehash: 744266ef8ffb17c4af4168d6239e5a5a30561936
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823570"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="0500b-103">genericError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0500b-103">genericError resource type</span></span>

> <span data-ttu-id="0500b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0500b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0500b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0500b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0500b-106">汎用のエラーです。</span><span class="sxs-lookup"><span data-stu-id="0500b-106">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="0500b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0500b-107">Properties</span></span>

| <span data-ttu-id="0500b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0500b-108">Property</span></span> | <span data-ttu-id="0500b-109">種類</span><span class="sxs-lookup"><span data-stu-id="0500b-109">Type</span></span> | <span data-ttu-id="0500b-110">説明</span><span class="sxs-lookup"><span data-stu-id="0500b-110">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="0500b-111">message</span><span class="sxs-lookup"><span data-stu-id="0500b-111">message</span></span> | <span data-ttu-id="0500b-112">String</span><span class="sxs-lookup"><span data-stu-id="0500b-112">String</span></span> | <span data-ttu-id="0500b-113">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="0500b-113">The error message.</span></span> |
| <span data-ttu-id="0500b-114">code</span><span class="sxs-lookup"><span data-stu-id="0500b-114">code</span></span> | <span data-ttu-id="0500b-115">String</span><span class="sxs-lookup"><span data-stu-id="0500b-115">String</span></span> | <span data-ttu-id="0500b-116">エラー コード。</span><span class="sxs-lookup"><span data-stu-id="0500b-116">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0500b-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0500b-117">JSON representation</span></span>

<span data-ttu-id="0500b-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0500b-118">Here is a JSON representation of the resource.</span></span>

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
