---
title: edgeSearchEngineBase リソースの種類
description: IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。 AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 63efe6e04c738bce5318a3792dccde08e5570cee
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332485"
---
# <a name="edgesearchenginebase-resource-type"></a><span data-ttu-id="b976e-104">edgeSearchEngineBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b976e-104">edgeSearchEngineBase resource type</span></span>

> <span data-ttu-id="b976e-105">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b976e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b976e-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b976e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b976e-107">IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="b976e-107">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="b976e-108">AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="b976e-108">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>

## <a name="properties"></a><span data-ttu-id="b976e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b976e-109">Properties</span></span>
|<span data-ttu-id="b976e-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b976e-110">Property</span></span>|<span data-ttu-id="b976e-111">型</span><span class="sxs-lookup"><span data-stu-id="b976e-111">Type</span></span>|<span data-ttu-id="b976e-112">説明</span><span class="sxs-lookup"><span data-stu-id="b976e-112">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="b976e-113">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b976e-113">Relationships</span></span>
<span data-ttu-id="b976e-114">なし</span><span class="sxs-lookup"><span data-stu-id="b976e-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b976e-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b976e-115">JSON Representation</span></span>
<span data-ttu-id="b976e-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b976e-116">Here is a JSON representation of the resource.</span></span>
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



