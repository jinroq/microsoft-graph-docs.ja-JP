---
title: mobileAppContent の作成
description: 新しい mobileAppContent オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 096d99b382e1942095522191b6275e019e8823d4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916426"
---
# <a name="create-mobileappcontent"></a><span data-ttu-id="fec29-103">mobileAppContent の作成</span><span class="sxs-lookup"><span data-stu-id="fec29-103">Create mobileAppContent</span></span>

> <span data-ttu-id="fec29-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fec29-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fec29-105">新しい [mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fec29-105">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fec29-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="fec29-106">Prerequisites</span></span>
<span data-ttu-id="fec29-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fec29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fec29-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fec29-109">Permission type</span></span>|<span data-ttu-id="fec29-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fec29-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fec29-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fec29-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fec29-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fec29-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fec29-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fec29-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fec29-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fec29-114">Not supported.</span></span>|
|<span data-ttu-id="fec29-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fec29-115">Application</span></span>|<span data-ttu-id="fec29-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fec29-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fec29-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fec29-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="fec29-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fec29-118">Request headers</span></span>
|<span data-ttu-id="fec29-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fec29-119">Header</span></span>|<span data-ttu-id="fec29-120">値</span><span class="sxs-lookup"><span data-stu-id="fec29-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fec29-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fec29-121">Authorization</span></span>|<span data-ttu-id="fec29-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fec29-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fec29-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fec29-123">Accept</span></span>|<span data-ttu-id="fec29-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fec29-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fec29-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="fec29-125">Request body</span></span>
<span data-ttu-id="fec29-126">要求本文で、mobileAppContent オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fec29-126">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="fec29-127">次の表に、mobileAppContent の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fec29-127">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="fec29-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fec29-128">Property</span></span>|<span data-ttu-id="fec29-129">種類</span><span class="sxs-lookup"><span data-stu-id="fec29-129">Type</span></span>|<span data-ttu-id="fec29-130">説明</span><span class="sxs-lookup"><span data-stu-id="fec29-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fec29-131">ID</span><span class="sxs-lookup"><span data-stu-id="fec29-131">id</span></span>|<span data-ttu-id="fec29-132">String</span><span class="sxs-lookup"><span data-stu-id="fec29-132">String</span></span>|<span data-ttu-id="fec29-133">アプリのコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="fec29-133">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="fec29-134">応答</span><span class="sxs-lookup"><span data-stu-id="fec29-134">Response</span></span>
<span data-ttu-id="fec29-135">成功した場合、このメソッドは `201 Created` 応答コードと応答本文で [mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fec29-135">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fec29-136">例</span><span class="sxs-lookup"><span data-stu-id="fec29-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="fec29-137">要求</span><span class="sxs-lookup"><span data-stu-id="fec29-137">Request</span></span>
<span data-ttu-id="fec29-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fec29-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="fec29-139">応答</span><span class="sxs-lookup"><span data-stu-id="fec29-139">Response</span></span>
<span data-ttu-id="fec29-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fec29-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```



