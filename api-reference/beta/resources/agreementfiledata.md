---
title: agreementFileData リソースの種類
description: Azure Active Directory の blob ファイルの使用許諾契約書の条項を (Azure AD) を表します。
localization_priority: Normal
ms.openlocfilehash: 64de3a72ad648225f24429987f5729f76ed8a2e7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815219"
---
# <a name="agreementfiledata-resource-type"></a><span data-ttu-id="0bea6-103">agreementFileData リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0bea6-103">agreementFileData resource type</span></span>

> <span data-ttu-id="0bea6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0bea6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0bea6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bea6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0bea6-106">Azure Active Directory の blob ファイルの使用許諾契約書の条項を (Azure AD) を表します。</span><span class="sxs-lookup"><span data-stu-id="0bea6-106">Represents the blob of an Azure Active Directory (Azure AD) terms of use agreement file.</span></span>

## <a name="properties"></a><span data-ttu-id="0bea6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0bea6-107">Properties</span></span>
| <span data-ttu-id="0bea6-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0bea6-108">Method</span></span>       | <span data-ttu-id="0bea6-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0bea6-109">Return Type</span></span> | <span data-ttu-id="0bea6-110">説明</span><span class="sxs-lookup"><span data-stu-id="0bea6-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0bea6-111">data</span><span class="sxs-lookup"><span data-stu-id="0bea6-111">data</span></span>|<span data-ttu-id="0bea6-112">Binary</span><span class="sxs-lookup"><span data-stu-id="0bea6-112">Binary</span></span>|<span data-ttu-id="0bea6-113">PDF 文書の使用の条件を表すデータです。</span><span class="sxs-lookup"><span data-stu-id="0bea6-113">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="0bea6-114">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0bea6-114">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0bea6-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0bea6-115">JSON representation</span></span>

<span data-ttu-id="0bea6-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0bea6-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileData"
}-->

```json
{
  "data": "Binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "agreementFileData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
