---
title: fileEncryptionInfo リソースの種類
description: ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5642c76e7d09d1113f2fccc68fc7b1db8ba0ffde
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931602"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="1766d-103">fileEncryptionInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1766d-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="1766d-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1766d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1766d-105">ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1766d-105">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="1766d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1766d-106">Properties</span></span>
|<span data-ttu-id="1766d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1766d-107">Property</span></span>|<span data-ttu-id="1766d-108">種類</span><span class="sxs-lookup"><span data-stu-id="1766d-108">Type</span></span>|<span data-ttu-id="1766d-109">説明</span><span class="sxs-lookup"><span data-stu-id="1766d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1766d-110">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="1766d-110">encryptionKey</span></span>|<span data-ttu-id="1766d-111">Binary</span><span class="sxs-lookup"><span data-stu-id="1766d-111">Binary</span></span>|<span data-ttu-id="1766d-112">ファイルのコンテンツを暗号化するために使用するキーです。</span><span class="sxs-lookup"><span data-stu-id="1766d-112">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="1766d-113">initializationVector</span><span class="sxs-lookup"><span data-stu-id="1766d-113">initializationVector</span></span>|<span data-ttu-id="1766d-114">Binary</span><span class="sxs-lookup"><span data-stu-id="1766d-114">Binary</span></span>|<span data-ttu-id="1766d-115">暗号化アルゴリズムに使用される初期化ベクトルです。</span><span class="sxs-lookup"><span data-stu-id="1766d-115">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="1766d-116">Mac</span><span class="sxs-lookup"><span data-stu-id="1766d-116">mac</span></span>|<span data-ttu-id="1766d-117">Binary</span><span class="sxs-lookup"><span data-stu-id="1766d-117">Binary</span></span>|<span data-ttu-id="1766d-118">暗号化されたファイル コンテンツのハッシュ + IV (コンテンツ ハッシュ) です。</span><span class="sxs-lookup"><span data-stu-id="1766d-118">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="1766d-119">macKey</span><span class="sxs-lookup"><span data-stu-id="1766d-119">macKey</span></span>|<span data-ttu-id="1766d-120">Binary</span><span class="sxs-lookup"><span data-stu-id="1766d-120">Binary</span></span>|<span data-ttu-id="1766d-121">Mac を取得するために使用するキーです。</span><span class="sxs-lookup"><span data-stu-id="1766d-121">The key used to get mac.</span></span>|
|<span data-ttu-id="1766d-122">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="1766d-122">profileIdentifier</span></span>|<span data-ttu-id="1766d-123">String</span><span class="sxs-lookup"><span data-stu-id="1766d-123">String</span></span>|<span data-ttu-id="1766d-124">プロファイルの識別子です。</span><span class="sxs-lookup"><span data-stu-id="1766d-124">The the profile identifier.</span></span>|
|<span data-ttu-id="1766d-125">fileDigest</span><span class="sxs-lookup"><span data-stu-id="1766d-125">fileDigest</span></span>|<span data-ttu-id="1766d-126">Binary</span><span class="sxs-lookup"><span data-stu-id="1766d-126">Binary</span></span>|<span data-ttu-id="1766d-127">暗号化される前のファイル ダイジェストです。</span><span class="sxs-lookup"><span data-stu-id="1766d-127">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="1766d-128">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="1766d-128">fileDigestAlgorithm</span></span>|<span data-ttu-id="1766d-129">String</span><span class="sxs-lookup"><span data-stu-id="1766d-129">String</span></span>|<span data-ttu-id="1766d-130">ファイル ダイジェストのアルゴリズムです。</span><span class="sxs-lookup"><span data-stu-id="1766d-130">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1766d-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1766d-131">Relationships</span></span>
<span data-ttu-id="1766d-132">なし</span><span class="sxs-lookup"><span data-stu-id="1766d-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1766d-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1766d-133">JSON Representation</span></span>
<span data-ttu-id="1766d-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1766d-134">Here is a JSON representation of the resource.</span></span>
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



