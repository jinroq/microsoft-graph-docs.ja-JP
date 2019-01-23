---
title: getEncryptionPublicKey 関数
description: アップル デバイスの登録プログラムを暗号化するために使用する公開キーのトークンを取得します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b2d2359f5bc6c13f094b9c8fbe6e302ab82d9147
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420599"
---
# <a name="getencryptionpublickey-function"></a><span data-ttu-id="5cd40-103">getEncryptionPublicKey 関数</span><span class="sxs-lookup"><span data-stu-id="5cd40-103">getEncryptionPublicKey function</span></span>

> <span data-ttu-id="5cd40-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5cd40-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5cd40-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5cd40-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5cd40-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5cd40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cd40-107">アップル デバイスの登録プログラムを暗号化するために使用する公開キーのトークンを取得します。</span><span class="sxs-lookup"><span data-stu-id="5cd40-107">Get a public key to use to encrypt the Apple device enrollment program token</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5cd40-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="5cd40-108">Prerequisites</span></span>
<span data-ttu-id="5cd40-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5cd40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5cd40-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5cd40-111">Permission type</span></span>|<span data-ttu-id="5cd40-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5cd40-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cd40-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5cd40-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5cd40-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5cd40-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="5cd40-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5cd40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cd40-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5cd40-116">Not supported.</span></span>|
|<span data-ttu-id="5cd40-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5cd40-117">Application</span></span>|<span data-ttu-id="5cd40-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5cd40-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cd40-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5cd40-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/getEncryptionPublicKey
```

## <a name="request-headers"></a><span data-ttu-id="5cd40-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5cd40-120">Request headers</span></span>
|<span data-ttu-id="5cd40-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5cd40-121">Header</span></span>|<span data-ttu-id="5cd40-122">値</span><span class="sxs-lookup"><span data-stu-id="5cd40-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cd40-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cd40-123">Authorization</span></span>|<span data-ttu-id="5cd40-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5cd40-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5cd40-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5cd40-125">Accept</span></span>|<span data-ttu-id="5cd40-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5cd40-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cd40-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5cd40-127">Request body</span></span>
<span data-ttu-id="5cd40-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5cd40-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5cd40-129">応答</span><span class="sxs-lookup"><span data-stu-id="5cd40-129">Response</span></span>
<span data-ttu-id="5cd40-130">成功した場合、この関数は `200 OK` 応答コードと、応答本文で String を返します。</span><span class="sxs-lookup"><span data-stu-id="5cd40-130">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cd40-131">例</span><span class="sxs-lookup"><span data-stu-id="5cd40-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5cd40-132">要求</span><span class="sxs-lookup"><span data-stu-id="5cd40-132">Request</span></span>
<span data-ttu-id="5cd40-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5cd40-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/getEncryptionPublicKey
```

### <a name="response"></a><span data-ttu-id="5cd40-134">応答</span><span class="sxs-lookup"><span data-stu-id="5cd40-134">Response</span></span>
<span data-ttu-id="5cd40-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5cd40-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 50

{
  "value": "Get Encryption Public Key value"
}
```




