---
title: リスト windowsPhone81ImportedPFXCertificateProfiles
description: WindowsPhone81ImportedPFXCertificateProfile オブジェクトのプロパティと関係を一覧表示します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6a715b9f61580abd81148df98a776c13def5822d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424239"
---
# <a name="list-windowsphone81importedpfxcertificateprofiles"></a><span data-ttu-id="80127-103">リスト windowsPhone81ImportedPFXCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="80127-103">List windowsPhone81ImportedPFXCertificateProfiles</span></span>

> <span data-ttu-id="80127-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="80127-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="80127-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80127-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80127-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="80127-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80127-107">[WindowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="80127-107">List properties and relationships of the [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80127-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="80127-108">Prerequisites</span></span>
<span data-ttu-id="80127-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="80127-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="80127-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="80127-111">Permission type</span></span>|<span data-ttu-id="80127-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="80127-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80127-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="80127-113">Delegated (work or school account)</span></span>|<span data-ttu-id="80127-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="80127-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="80127-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="80127-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80127-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80127-116">Not supported.</span></span>|
|<span data-ttu-id="80127-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="80127-117">Application</span></span>|<span data-ttu-id="80127-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80127-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80127-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="80127-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="80127-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="80127-120">Request headers</span></span>
|<span data-ttu-id="80127-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="80127-121">Header</span></span>|<span data-ttu-id="80127-122">値</span><span class="sxs-lookup"><span data-stu-id="80127-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80127-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="80127-123">Authorization</span></span>|<span data-ttu-id="80127-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="80127-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80127-125">Accept</span><span class="sxs-lookup"><span data-stu-id="80127-125">Accept</span></span>|<span data-ttu-id="80127-126">application/json</span><span class="sxs-lookup"><span data-stu-id="80127-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80127-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="80127-127">Request body</span></span>
<span data-ttu-id="80127-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="80127-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80127-129">応答</span><span class="sxs-lookup"><span data-stu-id="80127-129">Response</span></span>
<span data-ttu-id="80127-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="80127-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80127-131">例</span><span class="sxs-lookup"><span data-stu-id="80127-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="80127-132">要求</span><span class="sxs-lookup"><span data-stu-id="80127-132">Request</span></span>
<span data-ttu-id="80127-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="80127-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="80127-134">応答</span><span class="sxs-lookup"><span data-stu-id="80127-134">Response</span></span>
<span data-ttu-id="80127-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="80127-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 868

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81ImportedPFXCertificateProfile",
      "id": "08c7f847-f847-08c7-47f8-c70847f8c708",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "renewalThresholdPercentage": 10,
      "keyStorageProvider": "useTpmKspOtherwiseFail",
      "subjectNameFormat": "commonNameIncludingEmail",
      "subjectAlternativeNameType": "emailAddress",
      "certificateValidityPeriodValue": 14,
      "certificateValidityPeriodScale": "months",
      "intendedPurpose": "smimeEncryption"
    }
  ]
}
```




