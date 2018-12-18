---
title: macOSLobChildApp リソースの種類
description: バンドル パッケージに MacOS の LOB アプリケーションのプロパティが含まれています
author: tfitzmac
ms.openlocfilehash: e62305ea856d42847b49be306d20bde737152163
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309871"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="2cd72-103">macOSLobChildApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2cd72-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="2cd72-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2cd72-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2cd72-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2cd72-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2cd72-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2cd72-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2cd72-107">バンドル パッケージに MacOS の LOB アプリケーションのプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="2cd72-107">Contains properties the MacOS LOB App in a bundle package</span></span>
## <a name="properties"></a><span data-ttu-id="2cd72-108">Properties</span><span class="sxs-lookup"><span data-stu-id="2cd72-108">Properties</span></span>
|<span data-ttu-id="2cd72-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2cd72-109">Property</span></span>|<span data-ttu-id="2cd72-110">種類</span><span class="sxs-lookup"><span data-stu-id="2cd72-110">Type</span></span>|<span data-ttu-id="2cd72-111">説明</span><span class="sxs-lookup"><span data-stu-id="2cd72-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cd72-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="2cd72-112">bundleId</span></span>|<span data-ttu-id="2cd72-113">String</span><span class="sxs-lookup"><span data-stu-id="2cd72-113">String</span></span>|<span data-ttu-id="2cd72-114">ID 名。</span><span class="sxs-lookup"><span data-stu-id="2cd72-114">The Identity Name.</span></span>|
|<span data-ttu-id="2cd72-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="2cd72-115">buildNumber</span></span>|<span data-ttu-id="2cd72-116">String</span><span class="sxs-lookup"><span data-stu-id="2cd72-116">String</span></span>|<span data-ttu-id="2cd72-117">MacOS の基幹業務 (LoB) アプリケーションのビルド番号です。</span><span class="sxs-lookup"><span data-stu-id="2cd72-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="2cd72-118">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="2cd72-118">versionNumber</span></span>|<span data-ttu-id="2cd72-119">String</span><span class="sxs-lookup"><span data-stu-id="2cd72-119">String</span></span>|<span data-ttu-id="2cd72-120">MacOS の基幹業務 (LoB) アプリケーションのバージョン番号です。</span><span class="sxs-lookup"><span data-stu-id="2cd72-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2cd72-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2cd72-121">Relationships</span></span>
<span data-ttu-id="2cd72-122">なし</span><span class="sxs-lookup"><span data-stu-id="2cd72-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2cd72-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2cd72-123">JSON Representation</span></span>
<span data-ttu-id="2cd72-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2cd72-124">Here is a JSON representation of the resource.</span></span>
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





