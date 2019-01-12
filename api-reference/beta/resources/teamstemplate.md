---
title: teamsTemplate リソースの種類
description: TeamsTemplate エンティティをについて説明します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9bd5047950ed1ed3c57950d2c4b708a78b570649
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940086"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="76598-103">teamsTemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="76598-103">teamsTemplate resource type</span></span>

> <span data-ttu-id="76598-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="76598-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76598-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76598-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="76598-106">チーム テンプレートは、マイクロソフトのチームで[チーム](../resources/team.md)を作成するための青写真です。</span><span class="sxs-lookup"><span data-stu-id="76598-106">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="76598-107">テンプレートは、テンプレートを使用して作成された新しいチームの構造、設定、および準備する必要があるものコンテンツを指定します。</span><span class="sxs-lookup"><span data-stu-id="76598-107">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="76598-108">マイクロソフトは、基本テンプレートのスイートを提供していて、お客様が独自のカスタム テンプレートを保存できます。</span><span class="sxs-lookup"><span data-stu-id="76598-108">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="76598-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76598-109">Properties</span></span>

| <span data-ttu-id="76598-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76598-110">Property</span></span>            | <span data-ttu-id="76598-111">種類</span><span class="sxs-lookup"><span data-stu-id="76598-111">Type</span></span>     | <span data-ttu-id="76598-112">説明</span><span class="sxs-lookup"><span data-stu-id="76598-112">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="76598-113">ID</span><span class="sxs-lookup"><span data-stu-id="76598-113">id</span></span>                  | <span data-ttu-id="76598-114">String</span><span class="sxs-lookup"><span data-stu-id="76598-114">String</span></span>   | <span data-ttu-id="76598-115">テンプレートの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="76598-115">Unique identifier of the template.</span></span> <span data-ttu-id="76598-116">Null にすることはできません。</span><span class="sxs-lookup"><span data-stu-id="76598-116">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="76598-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="76598-117">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="76598-118">関連項目</span><span class="sxs-lookup"><span data-stu-id="76598-118">See also</span></span>

- [<span data-ttu-id="76598-119">チーム</span><span class="sxs-lookup"><span data-stu-id="76598-119">team</span></span>](team.md)

