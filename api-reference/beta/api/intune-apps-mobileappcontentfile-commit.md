---
title: commit アクション
description: 特定のアプリのファイルをコミットします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 30ce7aee558c544aee29f1843d296e5e39ea8340
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149064"
---
# <a name="commit-action"></a><span data-ttu-id="f4f5d-103">コミット アクション</span><span class="sxs-lookup"><span data-stu-id="f4f5d-103">commit action</span></span>

> <span data-ttu-id="f4f5d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4f5d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4f5d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f4f5d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4f5d-106">特定のアプリのファイルをコミットします。</span><span class="sxs-lookup"><span data-stu-id="f4f5d-106">Commits a file of a given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4f5d-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f4f5d-107">Prerequisites</span></span>
<span data-ttu-id="f4f5d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4f5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f4f5d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f4f5d-110">Permission type</span></span>|<span data-ttu-id="f4f5d-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f4f5d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4f5d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f4f5d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4f5d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4f5d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f4f5d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f4f5d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4f5d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4f5d-115">Not supported.</span></span>|
|<span data-ttu-id="f4f5d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f4f5d-116">Application</span></span>|<span data-ttu-id="f4f5d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4f5d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4f5d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f4f5d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit
```

## <a name="request-headers"></a><span data-ttu-id="f4f5d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f4f5d-119">Request headers</span></span>
|<span data-ttu-id="f4f5d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f4f5d-120">Header</span></span>|<span data-ttu-id="f4f5d-121">値</span><span class="sxs-lookup"><span data-stu-id="f4f5d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4f5d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4f5d-122">Authorization</span></span>|<span data-ttu-id="f4f5d-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f4f5d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4f5d-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f4f5d-124">Accept</span></span>|<span data-ttu-id="f4f5d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4f5d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4f5d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f4f5d-126">Request body</span></span>
<span data-ttu-id="f4f5d-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f4f5d-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f4f5d-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="f4f5d-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f4f5d-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4f5d-129">Property</span></span>|<span data-ttu-id="f4f5d-130">型</span><span class="sxs-lookup"><span data-stu-id="f4f5d-130">Type</span></span>|<span data-ttu-id="f4f5d-131">説明</span><span class="sxs-lookup"><span data-stu-id="f4f5d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4f5d-132">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="f4f5d-132">fileEncryptionInfo</span></span>|[<span data-ttu-id="f4f5d-133">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="f4f5d-133">fileEncryptionInfo</span></span>](../resources/intune-apps-fileencryptioninfo.md)|<span data-ttu-id="f4f5d-134">ファイル暗号化情報のパラメーター キーです。</span><span class="sxs-lookup"><span data-stu-id="f4f5d-134">File encryption info parameter key.</span></span>|



## <a name="response"></a><span data-ttu-id="f4f5d-135">応答</span><span class="sxs-lookup"><span data-stu-id="f4f5d-135">Response</span></span>
<span data-ttu-id="f4f5d-136">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="f4f5d-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f4f5d-137">例</span><span class="sxs-lookup"><span data-stu-id="f4f5d-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4f5d-138">要求</span><span class="sxs-lookup"><span data-stu-id="f4f5d-138">Request</span></span>
<span data-ttu-id="f4f5d-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f4f5d-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit

Content-type: application/json
Content-length: 399

{
  "fileEncryptionInfo": {
    "@odata.type": "microsoft.graph.fileEncryptionInfo",
    "encryptionKey": "ZW5jcnlwdGlvbktleQ==",
    "initializationVector": "aW5pdGlhbGl6YXRpb25WZWN0b3I=",
    "mac": "bWFj",
    "macKey": "bWFjS2V5",
    "profileIdentifier": "Profile Identifier value",
    "fileDigest": "ZmlsZURpZ2VzdA==",
    "fileDigestAlgorithm": "File Digest Algorithm value"
  }
}
```

### <a name="response"></a><span data-ttu-id="f4f5d-140">応答</span><span class="sxs-lookup"><span data-stu-id="f4f5d-140">Response</span></span>
<span data-ttu-id="f4f5d-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f4f5d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




