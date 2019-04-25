---
title: Get managedEBookAssignment
description: managedEBookAssignment オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 492945f542bb1640c95475071ca9769f778edd79
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524873"
---
# <a name="get-managedebookassignment"></a><span data-ttu-id="81f68-103">Get managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="81f68-103">Get managedEBookAssignment</span></span>

> <span data-ttu-id="81f68-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="81f68-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81f68-105">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="81f68-105">Read properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81f68-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="81f68-106">Prerequisites</span></span>
<span data-ttu-id="81f68-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="81f68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81f68-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="81f68-109">Permission type</span></span>|<span data-ttu-id="81f68-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="81f68-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81f68-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="81f68-111">Delegated (work or school account)</span></span>|<span data-ttu-id="81f68-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="81f68-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="81f68-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="81f68-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81f68-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81f68-114">Not supported.</span></span>|
|<span data-ttu-id="81f68-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="81f68-115">Application</span></span>|<span data-ttu-id="81f68-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81f68-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81f68-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="81f68-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81f68-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="81f68-118">Optional query parameters</span></span>
<span data-ttu-id="81f68-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="81f68-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="81f68-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="81f68-120">Request headers</span></span>
|<span data-ttu-id="81f68-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="81f68-121">Header</span></span>|<span data-ttu-id="81f68-122">値</span><span class="sxs-lookup"><span data-stu-id="81f68-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81f68-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="81f68-123">Authorization</span></span>|<span data-ttu-id="81f68-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="81f68-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81f68-125">承諾</span><span class="sxs-lookup"><span data-stu-id="81f68-125">Accept</span></span>|<span data-ttu-id="81f68-126">application/json</span><span class="sxs-lookup"><span data-stu-id="81f68-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81f68-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="81f68-127">Request body</span></span>
<span data-ttu-id="81f68-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="81f68-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81f68-129">応答</span><span class="sxs-lookup"><span data-stu-id="81f68-129">Response</span></span>
<span data-ttu-id="81f68-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="81f68-130">If successful, this method returns a `200 OK` response code and [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81f68-131">例</span><span class="sxs-lookup"><span data-stu-id="81f68-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="81f68-132">要求</span><span class="sxs-lookup"><span data-stu-id="81f68-132">Request</span></span>
<span data-ttu-id="81f68-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="81f68-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

### <a name="response"></a><span data-ttu-id="81f68-134">応答</span><span class="sxs-lookup"><span data-stu-id="81f68-134">Response</span></span>
<span data-ttu-id="81f68-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="81f68-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": {
    "@odata.type": "#microsoft.graph.managedEBookAssignment",
    "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    },
    "installIntent": "required"
  }
}
```



