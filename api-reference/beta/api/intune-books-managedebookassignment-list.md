---
title: managedEBookAssignments のリスト
description: managedEBookAssignment オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3da7288174bb222835a9900a6a94327eac1831be
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934195"
---
# <a name="list-managedebookassignments"></a><span data-ttu-id="9504e-103">managedEBookAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="9504e-103">List managedEBookAssignments</span></span>

> <span data-ttu-id="9504e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9504e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9504e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9504e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9504e-106">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="9504e-106">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9504e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="9504e-107">Prerequisites</span></span>
<span data-ttu-id="9504e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9504e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9504e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9504e-110">Permission type</span></span>|<span data-ttu-id="9504e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9504e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9504e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9504e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9504e-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9504e-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9504e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9504e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9504e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9504e-115">Not supported.</span></span>|
|<span data-ttu-id="9504e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9504e-116">Application</span></span>|<span data-ttu-id="9504e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9504e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9504e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9504e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="9504e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9504e-119">Request headers</span></span>
|<span data-ttu-id="9504e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9504e-120">Header</span></span>|<span data-ttu-id="9504e-121">値</span><span class="sxs-lookup"><span data-stu-id="9504e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9504e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9504e-122">Authorization</span></span>|<span data-ttu-id="9504e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="9504e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9504e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="9504e-124">Accept</span></span>|<span data-ttu-id="9504e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9504e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9504e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9504e-126">Request body</span></span>
<span data-ttu-id="9504e-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9504e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9504e-128">応答</span><span class="sxs-lookup"><span data-stu-id="9504e-128">Response</span></span>
<span data-ttu-id="9504e-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="9504e-129">If successful, this method returns a `200 OK` response code and a collection of [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9504e-130">例</span><span class="sxs-lookup"><span data-stu-id="9504e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9504e-131">要求</span><span class="sxs-lookup"><span data-stu-id="9504e-131">Request</span></span>
<span data-ttu-id="9504e-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9504e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

### <a name="response"></a><span data-ttu-id="9504e-133">応答</span><span class="sxs-lookup"><span data-stu-id="9504e-133">Response</span></span>
<span data-ttu-id="9504e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9504e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




