---
title: getencryptionpublickey 関数
description: Apple device enrollment program トークンを暗号化するために使用する公開キーを取得する
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd34c3e6e88d432601aacf6bd8c8df851c90baef
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965628"
---
# <a name="getencryptionpublickey-function"></a><span data-ttu-id="6a034-103">getencryptionpublickey 関数</span><span class="sxs-lookup"><span data-stu-id="6a034-103">getEncryptionPublicKey function</span></span>

> <span data-ttu-id="6a034-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a034-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a034-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a034-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a034-106">Apple device enrollment program トークンを暗号化するために使用する公開キーを取得する</span><span class="sxs-lookup"><span data-stu-id="6a034-106">Get a public key to use to encrypt the Apple device enrollment program token</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a034-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6a034-107">Prerequisites</span></span>
<span data-ttu-id="6a034-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a034-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a034-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6a034-110">Permission type</span></span>|<span data-ttu-id="6a034-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6a034-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a034-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6a034-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a034-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a034-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="6a034-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6a034-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a034-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a034-115">Not supported.</span></span>|
|<span data-ttu-id="6a034-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6a034-116">Application</span></span>|<span data-ttu-id="6a034-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a034-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a034-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6a034-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/getEncryptionPublicKey
```

## <a name="request-headers"></a><span data-ttu-id="6a034-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a034-119">Request headers</span></span>
|<span data-ttu-id="6a034-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a034-120">Header</span></span>|<span data-ttu-id="6a034-121">値</span><span class="sxs-lookup"><span data-stu-id="6a034-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a034-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a034-122">Authorization</span></span>|<span data-ttu-id="6a034-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a034-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a034-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6a034-124">Accept</span></span>|<span data-ttu-id="6a034-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a034-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a034-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6a034-126">Request body</span></span>
<span data-ttu-id="6a034-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6a034-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a034-128">応答</span><span class="sxs-lookup"><span data-stu-id="6a034-128">Response</span></span>
<span data-ttu-id="6a034-129">成功した場合、この関数`200 OK`は応答コードと、応答本文で文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="6a034-129">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a034-130">例</span><span class="sxs-lookup"><span data-stu-id="6a034-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a034-131">要求</span><span class="sxs-lookup"><span data-stu-id="6a034-131">Request</span></span>
<span data-ttu-id="6a034-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6a034-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/getEncryptionPublicKey
```

### <a name="response"></a><span data-ttu-id="6a034-133">応答</span><span class="sxs-lookup"><span data-stu-id="6a034-133">Response</span></span>
<span data-ttu-id="6a034-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6a034-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 50

{
  "value": "Get Encryption Public Key value"
}
```




