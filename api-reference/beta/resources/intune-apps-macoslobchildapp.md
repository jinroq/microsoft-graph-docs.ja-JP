---
title: macOSLobChildApp リソースの種類
description: バンドル パッケージに MacOS の LOB アプリケーションのプロパティが含まれています
ms.openlocfilehash: 6035e77843923eacbce8a1647de241fc79338766
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069898"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="aee39-103">macOSLobChildApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aee39-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="aee39-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="aee39-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aee39-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aee39-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aee39-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="aee39-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aee39-107">バンドル パッケージに MacOS の LOB アプリケーションのプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="aee39-107">Contains properties the MacOS LOB App in a bundle package</span></span>
## <a name="properties"></a><span data-ttu-id="aee39-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aee39-108">Properties</span></span>
|<span data-ttu-id="aee39-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aee39-109">Property</span></span>|<span data-ttu-id="aee39-110">型</span><span class="sxs-lookup"><span data-stu-id="aee39-110">Type</span></span>|<span data-ttu-id="aee39-111">説明</span><span class="sxs-lookup"><span data-stu-id="aee39-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aee39-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="aee39-112">bundleId</span></span>|<span data-ttu-id="aee39-113">String</span><span class="sxs-lookup"><span data-stu-id="aee39-113">String</span></span>|<span data-ttu-id="aee39-114">ID 名。</span><span class="sxs-lookup"><span data-stu-id="aee39-114">The Identity Name.</span></span>|
|<span data-ttu-id="aee39-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="aee39-115">buildNumber</span></span>|<span data-ttu-id="aee39-116">String</span><span class="sxs-lookup"><span data-stu-id="aee39-116">String</span></span>|<span data-ttu-id="aee39-117">MacOS の基幹業務 (LoB) アプリケーションのビルド番号です。</span><span class="sxs-lookup"><span data-stu-id="aee39-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="aee39-118">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="aee39-118">versionNumber</span></span>|<span data-ttu-id="aee39-119">String</span><span class="sxs-lookup"><span data-stu-id="aee39-119">String</span></span>|<span data-ttu-id="aee39-120">MacOS の基幹業務 (LoB) アプリケーションのバージョン番号です。</span><span class="sxs-lookup"><span data-stu-id="aee39-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aee39-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aee39-121">Relationships</span></span>
<span data-ttu-id="aee39-122">なし</span><span class="sxs-lookup"><span data-stu-id="aee39-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="aee39-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aee39-123">JSON Representation</span></span>
<span data-ttu-id="aee39-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aee39-124">Here is a JSON representation of the resource.</span></span>
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





