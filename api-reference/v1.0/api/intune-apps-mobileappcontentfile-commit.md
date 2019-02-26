---
title: commit アクション
description: 特定のアプリのファイルをコミットします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9171f5360a524cd6414295219e13b58505051931
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257548"
---
# <a name="commit-action"></a><span data-ttu-id="deb65-103">コミット アクション</span><span class="sxs-lookup"><span data-stu-id="deb65-103">commit action</span></span>

> <span data-ttu-id="deb65-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="deb65-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="deb65-105">特定のアプリのファイルをコミットします。</span><span class="sxs-lookup"><span data-stu-id="deb65-105">Commits a file of a given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="deb65-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="deb65-106">Prerequisites</span></span>
<span data-ttu-id="deb65-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="deb65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="deb65-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="deb65-109">Permission type</span></span>|<span data-ttu-id="deb65-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="deb65-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="deb65-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="deb65-111">Delegated (work or school account)</span></span>|<span data-ttu-id="deb65-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deb65-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="deb65-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="deb65-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="deb65-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="deb65-114">Not supported.</span></span>|
|<span data-ttu-id="deb65-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="deb65-115">Application</span></span>|<span data-ttu-id="deb65-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="deb65-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="deb65-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="deb65-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit
```

## <a name="request-headers"></a><span data-ttu-id="deb65-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="deb65-118">Request headers</span></span>
|<span data-ttu-id="deb65-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="deb65-119">Header</span></span>|<span data-ttu-id="deb65-120">値</span><span class="sxs-lookup"><span data-stu-id="deb65-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="deb65-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="deb65-121">Authorization</span></span>|<span data-ttu-id="deb65-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="deb65-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="deb65-123">承諾</span><span class="sxs-lookup"><span data-stu-id="deb65-123">Accept</span></span>|<span data-ttu-id="deb65-124">application/json</span><span class="sxs-lookup"><span data-stu-id="deb65-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="deb65-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="deb65-125">Request body</span></span>
<span data-ttu-id="deb65-126">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="deb65-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="deb65-127">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="deb65-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="deb65-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="deb65-128">Property</span></span>|<span data-ttu-id="deb65-129">型</span><span class="sxs-lookup"><span data-stu-id="deb65-129">Type</span></span>|<span data-ttu-id="deb65-130">説明</span><span class="sxs-lookup"><span data-stu-id="deb65-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="deb65-131">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="deb65-131">fileEncryptionInfo</span></span>|[<span data-ttu-id="deb65-132">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="deb65-132">fileEncryptionInfo</span></span>](../resources/intune-apps-fileencryptioninfo.md)|<span data-ttu-id="deb65-133">ファイル暗号化情報のパラメーター キーです。</span><span class="sxs-lookup"><span data-stu-id="deb65-133">File encryption info parameter key.</span></span>|



## <a name="response"></a><span data-ttu-id="deb65-134">応答</span><span class="sxs-lookup"><span data-stu-id="deb65-134">Response</span></span>
<span data-ttu-id="deb65-135">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="deb65-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="deb65-136">例</span><span class="sxs-lookup"><span data-stu-id="deb65-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="deb65-137">要求</span><span class="sxs-lookup"><span data-stu-id="deb65-137">Request</span></span>
<span data-ttu-id="deb65-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="deb65-138">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="deb65-139">応答</span><span class="sxs-lookup"><span data-stu-id="deb65-139">Response</span></span>
<span data-ttu-id="deb65-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="deb65-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



