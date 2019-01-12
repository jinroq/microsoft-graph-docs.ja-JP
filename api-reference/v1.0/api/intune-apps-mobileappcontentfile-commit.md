---
title: commit アクション
description: 特定のアプリのファイルをコミットします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0b225a74f3a273e9e5dda7752b94e4a445d9794c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952343"
---
# <a name="commit-action"></a><span data-ttu-id="b3736-103">commit アクション</span><span class="sxs-lookup"><span data-stu-id="b3736-103">commit action</span></span>

> <span data-ttu-id="b3736-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b3736-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3736-105">特定のアプリのファイルをコミットします。</span><span class="sxs-lookup"><span data-stu-id="b3736-105">Commits a file of a given app.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b3736-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="b3736-106">Prerequisites</span></span>
<span data-ttu-id="b3736-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b3736-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3736-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b3736-109">Permission type</span></span>|<span data-ttu-id="b3736-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b3736-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3736-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b3736-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b3736-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3736-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b3736-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b3736-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3736-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3736-114">Not supported.</span></span>|
|<span data-ttu-id="b3736-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b3736-115">Application</span></span>|<span data-ttu-id="b3736-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3736-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3736-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b3736-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit
```

## <a name="request-headers"></a><span data-ttu-id="b3736-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3736-118">Request headers</span></span>
|<span data-ttu-id="b3736-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b3736-119">Header</span></span>|<span data-ttu-id="b3736-120">値</span><span class="sxs-lookup"><span data-stu-id="b3736-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3736-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3736-121">Authorization</span></span>|<span data-ttu-id="b3736-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b3736-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3736-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b3736-123">Accept</span></span>|<span data-ttu-id="b3736-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b3736-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3736-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b3736-125">Request body</span></span>
<span data-ttu-id="b3736-126">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b3736-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b3736-127">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="b3736-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b3736-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3736-128">Property</span></span>|<span data-ttu-id="b3736-129">種類</span><span class="sxs-lookup"><span data-stu-id="b3736-129">Type</span></span>|<span data-ttu-id="b3736-130">説明</span><span class="sxs-lookup"><span data-stu-id="b3736-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3736-131">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="b3736-131">fileEncryptionInfo</span></span>|[<span data-ttu-id="b3736-132">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="b3736-132">fileEncryptionInfo</span></span>](../resources/intune-apps-fileencryptioninfo.md)|<span data-ttu-id="b3736-133">ファイル暗号化情報のパラメーター キーです。</span><span class="sxs-lookup"><span data-stu-id="b3736-133">File encryption info parameter key.</span></span>|



## <a name="response"></a><span data-ttu-id="b3736-134">応答</span><span class="sxs-lookup"><span data-stu-id="b3736-134">Response</span></span>
<span data-ttu-id="b3736-135">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="b3736-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b3736-136">例</span><span class="sxs-lookup"><span data-stu-id="b3736-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="b3736-137">要求</span><span class="sxs-lookup"><span data-stu-id="b3736-137">Request</span></span>
<span data-ttu-id="b3736-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b3736-138">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b3736-139">応答</span><span class="sxs-lookup"><span data-stu-id="b3736-139">Response</span></span>
<span data-ttu-id="b3736-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b3736-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



