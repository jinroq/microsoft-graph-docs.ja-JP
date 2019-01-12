---
title: macOSLobChildApp リソースの種類
description: バンドル パッケージに MacOS の LOB アプリケーションのプロパティが含まれています
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 43f207bb2cebccdd01c791694674c6fbf96b631f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954233"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="c3189-103">macOSLobChildApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c3189-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="c3189-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c3189-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3189-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3189-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c3189-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c3189-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c3189-107">バンドル パッケージに MacOS の LOB アプリケーションのプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="c3189-107">Contains properties the MacOS LOB App in a bundle package</span></span>
## <a name="properties"></a><span data-ttu-id="c3189-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3189-108">Properties</span></span>
|<span data-ttu-id="c3189-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3189-109">Property</span></span>|<span data-ttu-id="c3189-110">種類</span><span class="sxs-lookup"><span data-stu-id="c3189-110">Type</span></span>|<span data-ttu-id="c3189-111">説明</span><span class="sxs-lookup"><span data-stu-id="c3189-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3189-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="c3189-112">bundleId</span></span>|<span data-ttu-id="c3189-113">String</span><span class="sxs-lookup"><span data-stu-id="c3189-113">String</span></span>|<span data-ttu-id="c3189-114">ID 名。</span><span class="sxs-lookup"><span data-stu-id="c3189-114">The Identity Name.</span></span>|
|<span data-ttu-id="c3189-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="c3189-115">buildNumber</span></span>|<span data-ttu-id="c3189-116">String</span><span class="sxs-lookup"><span data-stu-id="c3189-116">String</span></span>|<span data-ttu-id="c3189-117">MacOS の基幹業務 (LoB) アプリケーションのビルド番号です。</span><span class="sxs-lookup"><span data-stu-id="c3189-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="c3189-118">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="c3189-118">versionNumber</span></span>|<span data-ttu-id="c3189-119">String</span><span class="sxs-lookup"><span data-stu-id="c3189-119">String</span></span>|<span data-ttu-id="c3189-120">MacOS の基幹業務 (LoB) アプリケーションのバージョン番号です。</span><span class="sxs-lookup"><span data-stu-id="c3189-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3189-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c3189-121">Relationships</span></span>
<span data-ttu-id="c3189-122">なし</span><span class="sxs-lookup"><span data-stu-id="c3189-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c3189-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c3189-123">JSON Representation</span></span>
<span data-ttu-id="c3189-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c3189-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLobChildApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobChildApp",
  "bundleId": "String",
  "buildNumber": "String",
  "versionNumber": "String"
}
```





