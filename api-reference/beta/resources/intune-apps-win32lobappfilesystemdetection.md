---
title: win32LobAppFileSystemDetection リソースの種類
description: Win32 アプリケーションを検出するためにファイルまたはフォルダーのパスが含まれています
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c901949295b1ff411dec5e9827b7991c922c2315
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958209"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a><span data-ttu-id="f2ea3-103">win32LobAppFileSystemDetection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f2ea3-103">win32LobAppFileSystemDetection resource type</span></span>

> <span data-ttu-id="f2ea3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f2ea3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2ea3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2ea3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2ea3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f2ea3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2ea3-107">Win32 アプリケーションを検出するためにファイルまたはフォルダーのパスが含まれています</span><span class="sxs-lookup"><span data-stu-id="f2ea3-107">Contains file or folder path to detect a Win32 App</span></span>

<span data-ttu-id="f2ea3-108">[Win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f2ea3-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f2ea3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2ea3-109">Properties</span></span>
|<span data-ttu-id="f2ea3-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2ea3-110">Property</span></span>|<span data-ttu-id="f2ea3-111">型</span><span class="sxs-lookup"><span data-stu-id="f2ea3-111">Type</span></span>|<span data-ttu-id="f2ea3-112">説明</span><span class="sxs-lookup"><span data-stu-id="f2ea3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2ea3-113">path</span><span class="sxs-lookup"><span data-stu-id="f2ea3-113">path</span></span>|<span data-ttu-id="f2ea3-114">String</span><span class="sxs-lookup"><span data-stu-id="f2ea3-114">String</span></span>|<span data-ttu-id="f2ea3-115">Win32 基幹業務 (LoB) アプリケーションを検出するためにファイルまたはフォルダーのパス</span><span class="sxs-lookup"><span data-stu-id="f2ea3-115">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="f2ea3-116">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="f2ea3-116">fileOrFolderName</span></span>|<span data-ttu-id="f2ea3-117">String</span><span class="sxs-lookup"><span data-stu-id="f2ea3-117">String</span></span>|<span data-ttu-id="f2ea3-118">Win32 基幹業務 (LoB) アプリケーションを検出するためにファイルまたはフォルダーの名前</span><span class="sxs-lookup"><span data-stu-id="f2ea3-118">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="f2ea3-119">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="f2ea3-119">check32BitOn64System</span></span>|<span data-ttu-id="f2ea3-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2ea3-120">Boolean</span></span>|<span data-ttu-id="f2ea3-121">このファイルまたはフォルダーは、64 ビット システムで 32 ビット アプリケーションをチェックするかどうかを示す値</span><span class="sxs-lookup"><span data-stu-id="f2ea3-121">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="f2ea3-122">detectionType</span><span class="sxs-lookup"><span data-stu-id="f2ea3-122">detectionType</span></span>|[<span data-ttu-id="f2ea3-123">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="f2ea3-123">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="f2ea3-124">ファイル システムの検出の種類。</span><span class="sxs-lookup"><span data-stu-id="f2ea3-124">The file system detection type.</span></span> <span data-ttu-id="f2ea3-125">使用可能な値: `notConfigured`、`exists`、`modifiedDate`、`createdDate`、`version`、`sizeInMB`。</span><span class="sxs-lookup"><span data-stu-id="f2ea3-125">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span></span>|
|<span data-ttu-id="f2ea3-126">operator</span><span class="sxs-lookup"><span data-stu-id="f2ea3-126">operator</span></span>|[<span data-ttu-id="f2ea3-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="f2ea3-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="f2ea3-128">ファイルまたは fodler を検出するための演算子です。</span><span class="sxs-lookup"><span data-stu-id="f2ea3-128">The operator for file or fodler detection.</span></span> <span data-ttu-id="f2ea3-129">可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。</span><span class="sxs-lookup"><span data-stu-id="f2ea3-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="f2ea3-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="f2ea3-130">detectionValue</span></span>|<span data-ttu-id="f2ea3-131">String</span><span class="sxs-lookup"><span data-stu-id="f2ea3-131">String</span></span>|<span data-ttu-id="f2ea3-132">ファイルまたはフォルダーの検出値</span><span class="sxs-lookup"><span data-stu-id="f2ea3-132">The file or folder detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2ea3-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f2ea3-133">Relationships</span></span>
<span data-ttu-id="f2ea3-134">なし</span><span class="sxs-lookup"><span data-stu-id="f2ea3-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f2ea3-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f2ea3-135">JSON Representation</span></span>
<span data-ttu-id="f2ea3-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f2ea3-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemDetection",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```





