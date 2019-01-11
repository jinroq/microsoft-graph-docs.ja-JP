---
title: edgeSearchEngineBase リソースの種類
description: IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。 AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cb27c8a6924600e5bf92da87fb9e71a70b7bc419
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882307"
---
# <a name="edgesearchenginebase-resource-type"></a><span data-ttu-id="fa2cc-104">edgeSearchEngineBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fa2cc-104">edgeSearchEngineBase resource type</span></span>

> <span data-ttu-id="fa2cc-105">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fa2cc-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa2cc-106">IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="fa2cc-106">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="fa2cc-107">AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="fa2cc-107">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>
## <a name="properties"></a><span data-ttu-id="fa2cc-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa2cc-108">Properties</span></span>
|<span data-ttu-id="fa2cc-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa2cc-109">Property</span></span>|<span data-ttu-id="fa2cc-110">種類</span><span class="sxs-lookup"><span data-stu-id="fa2cc-110">Type</span></span>|<span data-ttu-id="fa2cc-111">説明</span><span class="sxs-lookup"><span data-stu-id="fa2cc-111">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="fa2cc-112">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fa2cc-112">Relationships</span></span>
<span data-ttu-id="fa2cc-113">なし</span><span class="sxs-lookup"><span data-stu-id="fa2cc-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fa2cc-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fa2cc-114">JSON Representation</span></span>
<span data-ttu-id="fa2cc-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fa2cc-115">Here is a JSON representation of the resource.</span></span>
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



