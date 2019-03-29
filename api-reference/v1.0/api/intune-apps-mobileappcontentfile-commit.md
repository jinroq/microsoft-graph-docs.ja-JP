---
title: commit アクション
description: 特定のアプリのファイルをコミットします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5d242d0bbf5fe69ae67167cb293582cbfc165220
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984815"
---
# <a name="commit-action"></a><span data-ttu-id="418d8-103">コミット アクション</span><span class="sxs-lookup"><span data-stu-id="418d8-103">commit action</span></span>

> <span data-ttu-id="418d8-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="418d8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="418d8-105">特定のアプリのファイルをコミットします。</span><span class="sxs-lookup"><span data-stu-id="418d8-105">Commits a file of a given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="418d8-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="418d8-106">Prerequisites</span></span>
<span data-ttu-id="418d8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="418d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="418d8-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="418d8-109">Permission type</span></span>|<span data-ttu-id="418d8-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="418d8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="418d8-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="418d8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="418d8-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="418d8-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="418d8-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="418d8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="418d8-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="418d8-114">Not supported.</span></span>|
|<span data-ttu-id="418d8-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="418d8-115">Application</span></span>|<span data-ttu-id="418d8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="418d8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="418d8-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="418d8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit
```

## <a name="request-headers"></a><span data-ttu-id="418d8-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="418d8-118">Request headers</span></span>
|<span data-ttu-id="418d8-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="418d8-119">Header</span></span>|<span data-ttu-id="418d8-120">値</span><span class="sxs-lookup"><span data-stu-id="418d8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="418d8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="418d8-121">Authorization</span></span>|<span data-ttu-id="418d8-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="418d8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="418d8-123">承諾</span><span class="sxs-lookup"><span data-stu-id="418d8-123">Accept</span></span>|<span data-ttu-id="418d8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="418d8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="418d8-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="418d8-125">Request body</span></span>
<span data-ttu-id="418d8-126">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="418d8-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="418d8-127">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="418d8-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="418d8-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="418d8-128">Property</span></span>|<span data-ttu-id="418d8-129">型</span><span class="sxs-lookup"><span data-stu-id="418d8-129">Type</span></span>|<span data-ttu-id="418d8-130">説明</span><span class="sxs-lookup"><span data-stu-id="418d8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="418d8-131">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="418d8-131">fileEncryptionInfo</span></span>|[<span data-ttu-id="418d8-132">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="418d8-132">fileEncryptionInfo</span></span>](../resources/intune-apps-fileencryptioninfo.md)|<span data-ttu-id="418d8-133">ファイル暗号化情報のパラメーター キーです。</span><span class="sxs-lookup"><span data-stu-id="418d8-133">File encryption info parameter key.</span></span>|



## <a name="response"></a><span data-ttu-id="418d8-134">応答</span><span class="sxs-lookup"><span data-stu-id="418d8-134">Response</span></span>
<span data-ttu-id="418d8-135">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="418d8-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="418d8-136">例</span><span class="sxs-lookup"><span data-stu-id="418d8-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="418d8-137">要求</span><span class="sxs-lookup"><span data-stu-id="418d8-137">Request</span></span>
<span data-ttu-id="418d8-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="418d8-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit

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

### <a name="response"></a><span data-ttu-id="418d8-139">応答</span><span class="sxs-lookup"><span data-stu-id="418d8-139">Response</span></span>
<span data-ttu-id="418d8-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="418d8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



