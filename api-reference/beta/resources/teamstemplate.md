---
title: teamsTemplate リソースの種類
description: TeamsTemplate エンティティをについて説明します。
ms.openlocfilehash: 76b2921e884d38a57097789b1ba64df3309d141c
ms.sourcegitcommit: 12c6e82f1417022540e534ebadbd0e8d7fb5abde
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/08/2018
ms.locfileid: "27210155"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="1d421-103">teamsTemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1d421-103">teamsTemplate resource type</span></span>

> <span data-ttu-id="1d421-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1d421-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d421-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d421-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1d421-106">チーム テンプレートは、マイクロソフトのチームで[チーム](../resources/team.md)を作成するための青写真です。</span><span class="sxs-lookup"><span data-stu-id="1d421-106">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="1d421-107">テンプレートは、テンプレートを使用して作成された新しいチームの構造、設定、および準備する必要があるものコンテンツを指定します。</span><span class="sxs-lookup"><span data-stu-id="1d421-107">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="1d421-108">マイクロソフトは、基本テンプレートのスイートを提供していて、お客様が独自のカスタム テンプレートを保存できます。</span><span class="sxs-lookup"><span data-stu-id="1d421-108">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="1d421-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d421-109">Properties</span></span>

| <span data-ttu-id="1d421-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d421-110">Property</span></span>            | <span data-ttu-id="1d421-111">種類</span><span class="sxs-lookup"><span data-stu-id="1d421-111">Type</span></span>     | <span data-ttu-id="1d421-112">説明</span><span class="sxs-lookup"><span data-stu-id="1d421-112">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="1d421-113">id</span><span class="sxs-lookup"><span data-stu-id="1d421-113">id</span></span>                  | <span data-ttu-id="1d421-114">String</span><span class="sxs-lookup"><span data-stu-id="1d421-114">String</span></span>   | <span data-ttu-id="1d421-115">テンプレートの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="1d421-115">Unique identifier of the template.</span></span> <span data-ttu-id="1d421-116">Null にすることはできません。</span><span class="sxs-lookup"><span data-stu-id="1d421-116">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1d421-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1d421-117">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="1d421-118">関連項目</span><span class="sxs-lookup"><span data-stu-id="1d421-118">See also</span></span>

- [<span data-ttu-id="1d421-119">チーム</span><span class="sxs-lookup"><span data-stu-id="1d421-119">team</span></span>](team.md)

