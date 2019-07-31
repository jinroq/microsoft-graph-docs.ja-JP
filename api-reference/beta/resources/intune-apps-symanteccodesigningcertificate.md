---
title: symantecCodeSigningCertificate リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 99cdc636f0a8a5eb5381d09e7c3596bf3e41180d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012374"
---
# <a name="symanteccodesigningcertificate-resource-type"></a><span data-ttu-id="50685-103">symantecCodeSigningCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="50685-103">symantecCodeSigningCertificate resource type</span></span>

> <span data-ttu-id="50685-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50685-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50685-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="50685-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50685-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="50685-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="50685-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="50685-107">Methods</span></span>
|<span data-ttu-id="50685-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="50685-108">Method</span></span>|<span data-ttu-id="50685-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="50685-109">Return Type</span></span>|<span data-ttu-id="50685-110">説明</span><span class="sxs-lookup"><span data-stu-id="50685-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="50685-111">SymantecCodeSigningCertificate を取得する</span><span class="sxs-lookup"><span data-stu-id="50685-111">Get symantecCodeSigningCertificate</span></span>](../api/intune-apps-symanteccodesigningcertificate-get.md)|[<span data-ttu-id="50685-112">symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="50685-112">symantecCodeSigningCertificate</span></span>](../resources/intune-apps-symanteccodesigningcertificate.md)|<span data-ttu-id="50685-113">[SymantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="50685-113">Read properties and relationships of the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>|
|[<span data-ttu-id="50685-114">SymantecCodeSigningCertificate の更新</span><span class="sxs-lookup"><span data-stu-id="50685-114">Update symantecCodeSigningCertificate</span></span>](../api/intune-apps-symanteccodesigningcertificate-update.md)|[<span data-ttu-id="50685-115">symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="50685-115">symantecCodeSigningCertificate</span></span>](../resources/intune-apps-symanteccodesigningcertificate.md)|<span data-ttu-id="50685-116">[SymantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="50685-116">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="50685-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50685-117">Properties</span></span>
|<span data-ttu-id="50685-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50685-118">Property</span></span>|<span data-ttu-id="50685-119">型</span><span class="sxs-lookup"><span data-stu-id="50685-119">Type</span></span>|<span data-ttu-id="50685-120">説明</span><span class="sxs-lookup"><span data-stu-id="50685-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50685-121">id</span><span class="sxs-lookup"><span data-stu-id="50685-121">id</span></span>|<span data-ttu-id="50685-122">文字列</span><span class="sxs-lookup"><span data-stu-id="50685-122">String</span></span>|<span data-ttu-id="50685-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="50685-123">The key of the entity.</span></span>|
|<span data-ttu-id="50685-124">content</span><span class="sxs-lookup"><span data-stu-id="50685-124">content</span></span>|<span data-ttu-id="50685-125">Binary</span><span class="sxs-lookup"><span data-stu-id="50685-125">Binary</span></span>|<span data-ttu-id="50685-126">Windows Symantec コード署名証明書が生データ形式で表示されます。</span><span class="sxs-lookup"><span data-stu-id="50685-126">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="50685-127">status</span><span class="sxs-lookup"><span data-stu-id="50685-127">status</span></span>|[<span data-ttu-id="50685-128">certificateStatus</span><span class="sxs-lookup"><span data-stu-id="50685-128">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="50685-129">証明書の状態がプロビジョニングされているか、プロビジョニングされていません。</span><span class="sxs-lookup"><span data-stu-id="50685-129">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="50685-130">可能な値は、`notProvisioned`、`provisioned` です。</span><span class="sxs-lookup"><span data-stu-id="50685-130">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="50685-131">パスワード</span><span class="sxs-lookup"><span data-stu-id="50685-131">password</span></span>|<span data-ttu-id="50685-132">String</span><span class="sxs-lookup"><span data-stu-id="50685-132">String</span></span>|<span data-ttu-id="50685-133">.Pfx ファイルに必要なパスワードを指定します。</span><span class="sxs-lookup"><span data-stu-id="50685-133">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="50685-134">subjectName</span><span class="sxs-lookup"><span data-stu-id="50685-134">subjectName</span></span>|<span data-ttu-id="50685-135">String</span><span class="sxs-lookup"><span data-stu-id="50685-135">String</span></span>|<span data-ttu-id="50685-136">証明書のサブジェクト名。</span><span class="sxs-lookup"><span data-stu-id="50685-136">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="50685-137">subject</span><span class="sxs-lookup"><span data-stu-id="50685-137">subject</span></span>|<span data-ttu-id="50685-138">String</span><span class="sxs-lookup"><span data-stu-id="50685-138">String</span></span>|<span data-ttu-id="50685-139">証明書のサブジェクトの値。</span><span class="sxs-lookup"><span data-stu-id="50685-139">The Subject value for the cert.</span></span>|
|<span data-ttu-id="50685-140">issuerName</span><span class="sxs-lookup"><span data-stu-id="50685-140">issuerName</span></span>|<span data-ttu-id="50685-141">String</span><span class="sxs-lookup"><span data-stu-id="50685-141">String</span></span>|<span data-ttu-id="50685-142">証明書の発行者名。</span><span class="sxs-lookup"><span data-stu-id="50685-142">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="50685-143">会社</span><span class="sxs-lookup"><span data-stu-id="50685-143">issuer</span></span>|<span data-ttu-id="50685-144">String</span><span class="sxs-lookup"><span data-stu-id="50685-144">String</span></span>|<span data-ttu-id="50685-145">証明書の発行者の値。</span><span class="sxs-lookup"><span data-stu-id="50685-145">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="50685-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="50685-146">expirationDateTime</span></span>|<span data-ttu-id="50685-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50685-147">DateTimeOffset</span></span>|<span data-ttu-id="50685-148">証明書の有効期限。</span><span class="sxs-lookup"><span data-stu-id="50685-148">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="50685-149">uploadDateTime</span><span class="sxs-lookup"><span data-stu-id="50685-149">uploadDateTime</span></span>|<span data-ttu-id="50685-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50685-150">DateTimeOffset</span></span>|<span data-ttu-id="50685-151">Symantec Cert としての CodeSigning Cert の種類。</span><span class="sxs-lookup"><span data-stu-id="50685-151">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50685-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="50685-152">Relationships</span></span>
<span data-ttu-id="50685-153">なし</span><span class="sxs-lookup"><span data-stu-id="50685-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50685-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="50685-154">JSON Representation</span></span>
<span data-ttu-id="50685-155">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="50685-155">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.symantecCodeSigningCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "id": "String (identifier)",
  "content": "binary",
  "status": "String",
  "password": "String",
  "subjectName": "String",
  "subject": "String",
  "issuerName": "String",
  "issuer": "String",
  "expirationDateTime": "String (timestamp)",
  "uploadDateTime": "String (timestamp)"
}
```





