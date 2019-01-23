---
title: edgeSearchEngineBase リソースの種類
description: IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。 AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 30202e4be3c45f18dbcc3d010977baf97826a682
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392788"
---
# <a name="edgesearchenginebase-resource-type"></a><span data-ttu-id="7010a-104">edgeSearchEngineBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7010a-104">edgeSearchEngineBase resource type</span></span>

> <span data-ttu-id="7010a-105">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7010a-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7010a-106">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7010a-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7010a-107">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7010a-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7010a-108">IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="7010a-108">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="7010a-109">AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="7010a-109">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>

## <a name="properties"></a><span data-ttu-id="7010a-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7010a-110">Properties</span></span>
|<span data-ttu-id="7010a-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7010a-111">Property</span></span>|<span data-ttu-id="7010a-112">型</span><span class="sxs-lookup"><span data-stu-id="7010a-112">Type</span></span>|<span data-ttu-id="7010a-113">説明</span><span class="sxs-lookup"><span data-stu-id="7010a-113">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="7010a-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7010a-114">Relationships</span></span>
<span data-ttu-id="7010a-115">なし</span><span class="sxs-lookup"><span data-stu-id="7010a-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7010a-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7010a-116">JSON Representation</span></span>
<span data-ttu-id="7010a-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7010a-117">Here is a JSON representation of the resource.</span></span>
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




