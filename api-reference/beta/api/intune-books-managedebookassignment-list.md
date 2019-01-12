---
title: managedEBookAssignments のリスト
description: managedEBookAssignment オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c1663ce272bc5dc94dfc77034354cf57ba615faa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968263"
---
# <a name="list-managedebookassignments"></a><span data-ttu-id="abcdc-103">managedEBookAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="abcdc-103">List managedEBookAssignments</span></span>

> <span data-ttu-id="abcdc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="abcdc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="abcdc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abcdc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="abcdc-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="abcdc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="abcdc-107">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="abcdc-107">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="abcdc-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="abcdc-108">Prerequisites</span></span>
<span data-ttu-id="abcdc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="abcdc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abcdc-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="abcdc-111">Permission type</span></span>|<span data-ttu-id="abcdc-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="abcdc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abcdc-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="abcdc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="abcdc-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="abcdc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="abcdc-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="abcdc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abcdc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abcdc-116">Not supported.</span></span>|
|<span data-ttu-id="abcdc-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="abcdc-117">Application</span></span>|<span data-ttu-id="abcdc-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abcdc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abcdc-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="abcdc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="abcdc-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="abcdc-120">Request headers</span></span>
|<span data-ttu-id="abcdc-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="abcdc-121">Header</span></span>|<span data-ttu-id="abcdc-122">値</span><span class="sxs-lookup"><span data-stu-id="abcdc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abcdc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="abcdc-123">Authorization</span></span>|<span data-ttu-id="abcdc-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="abcdc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abcdc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="abcdc-125">Accept</span></span>|<span data-ttu-id="abcdc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="abcdc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abcdc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="abcdc-127">Request body</span></span>
<span data-ttu-id="abcdc-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="abcdc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abcdc-129">応答</span><span class="sxs-lookup"><span data-stu-id="abcdc-129">Response</span></span>
<span data-ttu-id="abcdc-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="abcdc-130">If successful, this method returns a `200 OK` response code and a collection of [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abcdc-131">例</span><span class="sxs-lookup"><span data-stu-id="abcdc-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="abcdc-132">要求</span><span class="sxs-lookup"><span data-stu-id="abcdc-132">Request</span></span>
<span data-ttu-id="abcdc-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="abcdc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

### <a name="response"></a><span data-ttu-id="abcdc-134">応答</span><span class="sxs-lookup"><span data-stu-id="abcdc-134">Response</span></span>
<span data-ttu-id="abcdc-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="abcdc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 300

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedEBookAssignment",
      "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "installIntent": "required"
    }
  ]
}
```





