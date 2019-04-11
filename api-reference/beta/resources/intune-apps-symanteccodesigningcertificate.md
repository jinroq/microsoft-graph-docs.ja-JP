---
title: symantecCodeSigningCertificate リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 03f028dffe4db6a2e43a90d708bc16c61615a6a0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804453"
---
# <a name="symanteccodesigningcertificate-resource-type"></a><span data-ttu-id="2fa19-103">symantecCodeSigningCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2fa19-103">symantecCodeSigningCertificate resource type</span></span>

> <span data-ttu-id="2fa19-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2fa19-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2fa19-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2fa19-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fa19-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="2fa19-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="2fa19-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="2fa19-107">Methods</span></span>
|<span data-ttu-id="2fa19-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="2fa19-108">Method</span></span>|<span data-ttu-id="2fa19-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2fa19-109">Return Type</span></span>|<span data-ttu-id="2fa19-110">説明</span><span class="sxs-lookup"><span data-stu-id="2fa19-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2fa19-111">symantecCodeSigningCertificate を取得する</span><span class="sxs-lookup"><span data-stu-id="2fa19-111">Get symantecCodeSigningCertificate</span></span>](../api/intune-apps-symanteccodesigningcertificate-get.md)|[<span data-ttu-id="2fa19-112">symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="2fa19-112">symantecCodeSigningCertificate</span></span>](../resources/intune-apps-symanteccodesigningcertificate.md)|<span data-ttu-id="2fa19-113">[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2fa19-113">Read properties and relationships of the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>|
|[<span data-ttu-id="2fa19-114">symantecCodeSigningCertificate の更新</span><span class="sxs-lookup"><span data-stu-id="2fa19-114">Update symantecCodeSigningCertificate</span></span>](../api/intune-apps-symanteccodesigningcertificate-update.md)|[<span data-ttu-id="2fa19-115">symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="2fa19-115">symantecCodeSigningCertificate</span></span>](../resources/intune-apps-symanteccodesigningcertificate.md)|<span data-ttu-id="2fa19-116">[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2fa19-116">Update the properties of a [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2fa19-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2fa19-117">Properties</span></span>
|<span data-ttu-id="2fa19-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2fa19-118">Property</span></span>|<span data-ttu-id="2fa19-119">型</span><span class="sxs-lookup"><span data-stu-id="2fa19-119">Type</span></span>|<span data-ttu-id="2fa19-120">説明</span><span class="sxs-lookup"><span data-stu-id="2fa19-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fa19-121">id</span><span class="sxs-lookup"><span data-stu-id="2fa19-121">id</span></span>|<span data-ttu-id="2fa19-122">String</span><span class="sxs-lookup"><span data-stu-id="2fa19-122">String</span></span>|<span data-ttu-id="2fa19-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2fa19-123">The key of the entity.</span></span>|
|<span data-ttu-id="2fa19-124">content</span><span class="sxs-lookup"><span data-stu-id="2fa19-124">content</span></span>|<span data-ttu-id="2fa19-125">Binary</span><span class="sxs-lookup"><span data-stu-id="2fa19-125">Binary</span></span>|<span data-ttu-id="2fa19-126">Windows Symantec コード署名証明書が生データ形式で表示されます。</span><span class="sxs-lookup"><span data-stu-id="2fa19-126">The Windows Symantec Code-Signing Certificate in the raw data format.</span></span>|
|<span data-ttu-id="2fa19-127">status</span><span class="sxs-lookup"><span data-stu-id="2fa19-127">status</span></span>|[<span data-ttu-id="2fa19-128">certificatestatus</span><span class="sxs-lookup"><span data-stu-id="2fa19-128">certificateStatus</span></span>](../resources/intune-apps-certificatestatus.md)|<span data-ttu-id="2fa19-129">証明書の状態がプロビジョニングされているか、プロビジョニングされていません。</span><span class="sxs-lookup"><span data-stu-id="2fa19-129">The Cert Status Provisioned or not Provisioned.</span></span> <span data-ttu-id="2fa19-130">可能な値は、`notProvisioned`、`provisioned` です。</span><span class="sxs-lookup"><span data-stu-id="2fa19-130">Possible values are: `notProvisioned`, `provisioned`.</span></span>|
|<span data-ttu-id="2fa19-131">password</span><span class="sxs-lookup"><span data-stu-id="2fa19-131">password</span></span>|<span data-ttu-id="2fa19-132">String</span><span class="sxs-lookup"><span data-stu-id="2fa19-132">String</span></span>|<span data-ttu-id="2fa19-133">.pfx ファイルに必要なパスワードを指定します。</span><span class="sxs-lookup"><span data-stu-id="2fa19-133">The Password required for .pfx file.</span></span>|
|<span data-ttu-id="2fa19-134">subjectName</span><span class="sxs-lookup"><span data-stu-id="2fa19-134">subjectName</span></span>|<span data-ttu-id="2fa19-135">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2fa19-135">String</span></span>|<span data-ttu-id="2fa19-136">証明書のサブジェクト名。</span><span class="sxs-lookup"><span data-stu-id="2fa19-136">The Subject Name for the cert.</span></span>|
|<span data-ttu-id="2fa19-137">subject</span><span class="sxs-lookup"><span data-stu-id="2fa19-137">subject</span></span>|<span data-ttu-id="2fa19-138">String</span><span class="sxs-lookup"><span data-stu-id="2fa19-138">String</span></span>|<span data-ttu-id="2fa19-139">証明書のサブジェクトの値。</span><span class="sxs-lookup"><span data-stu-id="2fa19-139">The Subject value for the cert.</span></span>|
|<span data-ttu-id="2fa19-140">issuerName</span><span class="sxs-lookup"><span data-stu-id="2fa19-140">issuerName</span></span>|<span data-ttu-id="2fa19-141">文字列</span><span class="sxs-lookup"><span data-stu-id="2fa19-141">String</span></span>|<span data-ttu-id="2fa19-142">証明書の発行者名。</span><span class="sxs-lookup"><span data-stu-id="2fa19-142">The Issuer Name for the cert.</span></span>|
|<span data-ttu-id="2fa19-143">会社</span><span class="sxs-lookup"><span data-stu-id="2fa19-143">issuer</span></span>|<span data-ttu-id="2fa19-144">文字列</span><span class="sxs-lookup"><span data-stu-id="2fa19-144">String</span></span>|<span data-ttu-id="2fa19-145">証明書の発行者の値。</span><span class="sxs-lookup"><span data-stu-id="2fa19-145">The Issuer value for the cert.</span></span>|
|<span data-ttu-id="2fa19-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2fa19-146">expirationDateTime</span></span>|<span data-ttu-id="2fa19-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fa19-147">DateTimeOffset</span></span>|<span data-ttu-id="2fa19-148">証明書の有効期限。</span><span class="sxs-lookup"><span data-stu-id="2fa19-148">The Cert Expiration Date.</span></span>|
|<span data-ttu-id="2fa19-149">uploaddatetime</span><span class="sxs-lookup"><span data-stu-id="2fa19-149">uploadDateTime</span></span>|<span data-ttu-id="2fa19-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fa19-150">DateTimeOffset</span></span>|<span data-ttu-id="2fa19-151">Symantec cert としての CodeSigning cert の種類。</span><span class="sxs-lookup"><span data-stu-id="2fa19-151">The Type of the CodeSigning Cert as Symantec Cert.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fa19-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2fa19-152">Relationships</span></span>
<span data-ttu-id="2fa19-153">なし</span><span class="sxs-lookup"><span data-stu-id="2fa19-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2fa19-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2fa19-154">JSON Representation</span></span>
<span data-ttu-id="2fa19-155">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2fa19-155">Here is a JSON representation of the resource.</span></span>
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





