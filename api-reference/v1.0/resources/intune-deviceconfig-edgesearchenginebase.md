---
title: edgeSearchEngineBase リソースの種類
description: IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。 AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f2aeffb922ebf8b3a166b8f942d4159fa3fe7a3b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253324"
---
# <a name="edgesearchenginebase-resource-type"></a><span data-ttu-id="437f6-104">edgeSearchEngineBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="437f6-104">edgeSearchEngineBase resource type</span></span>

> <span data-ttu-id="437f6-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="437f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="437f6-106">IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="437f6-106">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="437f6-107">AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="437f6-107">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>

## <a name="properties"></a><span data-ttu-id="437f6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="437f6-108">Properties</span></span>
|<span data-ttu-id="437f6-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="437f6-109">Property</span></span>|<span data-ttu-id="437f6-110">型</span><span class="sxs-lookup"><span data-stu-id="437f6-110">Type</span></span>|<span data-ttu-id="437f6-111">説明</span><span class="sxs-lookup"><span data-stu-id="437f6-111">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="437f6-112">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="437f6-112">Relationships</span></span>
<span data-ttu-id="437f6-113">なし</span><span class="sxs-lookup"><span data-stu-id="437f6-113">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="437f6-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="437f6-114">JSON Representation</span></span>
<span data-ttu-id="437f6-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="437f6-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineBase"
}
```



