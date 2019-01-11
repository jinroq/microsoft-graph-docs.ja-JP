---
title: teamsTemplate リソースの種類
description: TeamsTemplate エンティティをについて説明します。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 6e847c7ef0b13dd9c4281c17939164128be8b6a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818873"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="399c9-103">teamsTemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="399c9-103">teamsTemplate resource type</span></span>

> <span data-ttu-id="399c9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="399c9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="399c9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="399c9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="399c9-106">チーム テンプレートは、マイクロソフトのチームで[チーム](../resources/team.md)を作成するための青写真です。</span><span class="sxs-lookup"><span data-stu-id="399c9-106">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="399c9-107">テンプレートは、テンプレートを使用して作成された新しいチームの構造、設定、および準備する必要があるものコンテンツを指定します。</span><span class="sxs-lookup"><span data-stu-id="399c9-107">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="399c9-108">マイクロソフトは、基本テンプレートのスイートを提供していて、お客様が独自のカスタム テンプレートを保存できます。</span><span class="sxs-lookup"><span data-stu-id="399c9-108">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="399c9-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="399c9-109">Properties</span></span>

| <span data-ttu-id="399c9-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="399c9-110">Property</span></span>            | <span data-ttu-id="399c9-111">種類</span><span class="sxs-lookup"><span data-stu-id="399c9-111">Type</span></span>     | <span data-ttu-id="399c9-112">説明</span><span class="sxs-lookup"><span data-stu-id="399c9-112">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="399c9-113">ID</span><span class="sxs-lookup"><span data-stu-id="399c9-113">id</span></span>                  | <span data-ttu-id="399c9-114">String</span><span class="sxs-lookup"><span data-stu-id="399c9-114">String</span></span>   | <span data-ttu-id="399c9-115">テンプレートの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="399c9-115">Unique identifier of the template.</span></span> <span data-ttu-id="399c9-116">Null にすることはできません。</span><span class="sxs-lookup"><span data-stu-id="399c9-116">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="399c9-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="399c9-117">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTemplate",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

# <a name="see-also"></a><span data-ttu-id="399c9-118">関連項目</span><span class="sxs-lookup"><span data-stu-id="399c9-118">See also</span></span>

- [<span data-ttu-id="399c9-119">チーム</span><span class="sxs-lookup"><span data-stu-id="399c9-119">team</span></span>](team.md)

