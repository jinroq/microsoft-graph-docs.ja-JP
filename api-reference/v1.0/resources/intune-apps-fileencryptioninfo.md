---
title: fileEncryptionInfo リソースの種類
description: ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a6aa144db5b4bc06177af77b965a6268d199105a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029191"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="13658-103">fileEncryptionInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="13658-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="13658-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="13658-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13658-105">ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="13658-105">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="13658-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13658-106">Properties</span></span>
|<span data-ttu-id="13658-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13658-107">Property</span></span>|<span data-ttu-id="13658-108">型</span><span class="sxs-lookup"><span data-stu-id="13658-108">Type</span></span>|<span data-ttu-id="13658-109">説明</span><span class="sxs-lookup"><span data-stu-id="13658-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13658-110">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="13658-110">encryptionKey</span></span>|<span data-ttu-id="13658-111">Binary</span><span class="sxs-lookup"><span data-stu-id="13658-111">Binary</span></span>|<span data-ttu-id="13658-112">ファイルのコンテンツを暗号化するために使用するキーです。</span><span class="sxs-lookup"><span data-stu-id="13658-112">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="13658-113">initializationVector</span><span class="sxs-lookup"><span data-stu-id="13658-113">initializationVector</span></span>|<span data-ttu-id="13658-114">Binary</span><span class="sxs-lookup"><span data-stu-id="13658-114">Binary</span></span>|<span data-ttu-id="13658-115">暗号化アルゴリズムに使用される初期化ベクトルです。</span><span class="sxs-lookup"><span data-stu-id="13658-115">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="13658-116">Mac</span><span class="sxs-lookup"><span data-stu-id="13658-116">mac</span></span>|<span data-ttu-id="13658-117">Binary</span><span class="sxs-lookup"><span data-stu-id="13658-117">Binary</span></span>|<span data-ttu-id="13658-118">暗号化されたファイル コンテンツのハッシュ + IV (コンテンツ ハッシュ) です。</span><span class="sxs-lookup"><span data-stu-id="13658-118">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="13658-119">macKey</span><span class="sxs-lookup"><span data-stu-id="13658-119">macKey</span></span>|<span data-ttu-id="13658-120">Binary</span><span class="sxs-lookup"><span data-stu-id="13658-120">Binary</span></span>|<span data-ttu-id="13658-121">Mac を取得するために使用するキーです。</span><span class="sxs-lookup"><span data-stu-id="13658-121">The key used to get mac.</span></span>|
|<span data-ttu-id="13658-122">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="13658-122">profileIdentifier</span></span>|<span data-ttu-id="13658-123">String</span><span class="sxs-lookup"><span data-stu-id="13658-123">String</span></span>|<span data-ttu-id="13658-124">プロファイル識別子。</span><span class="sxs-lookup"><span data-stu-id="13658-124">The profile identifier.</span></span>|
|<span data-ttu-id="13658-125">fileDigest</span><span class="sxs-lookup"><span data-stu-id="13658-125">fileDigest</span></span>|<span data-ttu-id="13658-126">Binary</span><span class="sxs-lookup"><span data-stu-id="13658-126">Binary</span></span>|<span data-ttu-id="13658-127">暗号化される前のファイル ダイジェストです。</span><span class="sxs-lookup"><span data-stu-id="13658-127">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="13658-128">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="13658-128">fileDigestAlgorithm</span></span>|<span data-ttu-id="13658-129">String</span><span class="sxs-lookup"><span data-stu-id="13658-129">String</span></span>|<span data-ttu-id="13658-130">ファイル ダイジェストのアルゴリズムです。</span><span class="sxs-lookup"><span data-stu-id="13658-130">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13658-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="13658-131">Relationships</span></span>
<span data-ttu-id="13658-132">なし</span><span class="sxs-lookup"><span data-stu-id="13658-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13658-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="13658-133">JSON Representation</span></span>
<span data-ttu-id="13658-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="13658-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileEncryptionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileEncryptionInfo",
  "encryptionKey": "binary",
  "initializationVector": "binary",
  "mac": "binary",
  "macKey": "binary",
  "profileIdentifier": "String",
  "fileDigest": "binary",
  "fileDigestAlgorithm": "String"
}
```



