---
title: edgeSearchEngineBase リソースの種類
description: IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。 AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2d4e039372338e2882ee226b5546592e0cfbd42e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924777"
---
# <a name="edgesearchenginebase-resource-type"></a><span data-ttu-id="f66da-104">edgeSearchEngineBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f66da-104">edgeSearchEngineBase resource type</span></span>

> <span data-ttu-id="f66da-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f66da-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f66da-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f66da-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f66da-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f66da-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f66da-108">IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="f66da-108">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="f66da-109">AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="f66da-109">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>
## <a name="properties"></a><span data-ttu-id="f66da-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f66da-110">Properties</span></span>
|<span data-ttu-id="f66da-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f66da-111">Property</span></span>|<span data-ttu-id="f66da-112">種類</span><span class="sxs-lookup"><span data-stu-id="f66da-112">Type</span></span>|<span data-ttu-id="f66da-113">説明</span><span class="sxs-lookup"><span data-stu-id="f66da-113">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="f66da-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f66da-114">Relationships</span></span>
<span data-ttu-id="f66da-115">なし</span><span class="sxs-lookup"><span data-stu-id="f66da-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f66da-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f66da-116">JSON Representation</span></span>
<span data-ttu-id="f66da-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f66da-117">Here is a JSON representation of the resource.</span></span>
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





