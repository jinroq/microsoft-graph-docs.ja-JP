---
title: userInstallStateSummaries のリスト
description: userInstallStateSummary オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e7f2eee3154900da9bb98c3fe28bb4f3dc4ca247
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934111"
---
# <a name="list-userinstallstatesummaries"></a><span data-ttu-id="43273-103">userInstallStateSummaries のリスト</span><span class="sxs-lookup"><span data-stu-id="43273-103">List userInstallStateSummaries</span></span>

> <span data-ttu-id="43273-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43273-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43273-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="43273-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43273-106">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="43273-106">List properties and relationships of the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43273-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="43273-107">Prerequisites</span></span>
<span data-ttu-id="43273-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="43273-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43273-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="43273-110">Permission type</span></span>|<span data-ttu-id="43273-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="43273-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43273-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="43273-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43273-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="43273-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="43273-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="43273-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43273-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43273-115">Not supported.</span></span>|
|<span data-ttu-id="43273-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="43273-116">Application</span></span>|<span data-ttu-id="43273-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43273-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43273-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="43273-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="43273-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43273-119">Request headers</span></span>
|<span data-ttu-id="43273-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43273-120">Header</span></span>|<span data-ttu-id="43273-121">値</span><span class="sxs-lookup"><span data-stu-id="43273-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43273-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="43273-122">Authorization</span></span>|<span data-ttu-id="43273-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="43273-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43273-124">承諾</span><span class="sxs-lookup"><span data-stu-id="43273-124">Accept</span></span>|<span data-ttu-id="43273-125">application/json</span><span class="sxs-lookup"><span data-stu-id="43273-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43273-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="43273-126">Request body</span></span>
<span data-ttu-id="43273-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="43273-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43273-128">応答</span><span class="sxs-lookup"><span data-stu-id="43273-128">Response</span></span>
<span data-ttu-id="43273-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="43273-129">If successful, this method returns a `200 OK` response code and a collection of [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43273-130">例</span><span class="sxs-lookup"><span data-stu-id="43273-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="43273-131">要求</span><span class="sxs-lookup"><span data-stu-id="43273-131">Request</span></span>
<span data-ttu-id="43273-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="43273-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

### <a name="response"></a><span data-ttu-id="43273-133">応答</span><span class="sxs-lookup"><span data-stu-id="43273-133">Response</span></span>
<span data-ttu-id="43273-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="43273-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 295

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userInstallStateSummary",
      "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
      "userName": "User Name value",
      "installedDeviceCount": 4,
      "failedDeviceCount": 1,
      "notInstalledDeviceCount": 7
    }
  ]
}
```




