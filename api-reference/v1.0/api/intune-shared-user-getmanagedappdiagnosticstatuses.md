---
title: getManagedAppDiagnosticStatuses 関数
description: 特定のユーザーの診断検証状態を取得します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8af90447f721d559c5620af58e30600b1ce29b11
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576676"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="27499-103">getManagedAppDiagnosticStatuses 関数</span><span class="sxs-lookup"><span data-stu-id="27499-103">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="27499-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="27499-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27499-105">特定のユーザーの診断検証状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="27499-105">Gets diagnostics validation status for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27499-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="27499-106">Prerequisites</span></span>
<span data-ttu-id="27499-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="27499-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27499-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="27499-109">Permission type</span></span>|<span data-ttu-id="27499-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="27499-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27499-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="27499-111">Delegated (work or school account)</span></span>| <span data-ttu-id="27499-112">_コンテキストによって異なる_</span><span class="sxs-lookup"><span data-stu-id="27499-112">_varies by context_</span></span>|
| <span data-ttu-id="27499-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="27499-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="27499-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="27499-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="27499-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="27499-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27499-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27499-116">Not supported.</span></span>|
|<span data-ttu-id="27499-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="27499-117">Application</span></span>|<span data-ttu-id="27499-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27499-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27499-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="27499-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="27499-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27499-120">Request headers</span></span>
|<span data-ttu-id="27499-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27499-121">Header</span></span>|<span data-ttu-id="27499-122">値</span><span class="sxs-lookup"><span data-stu-id="27499-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27499-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="27499-123">Authorization</span></span>|<span data-ttu-id="27499-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="27499-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27499-125">承諾</span><span class="sxs-lookup"><span data-stu-id="27499-125">Accept</span></span>|<span data-ttu-id="27499-126">application/json</span><span class="sxs-lookup"><span data-stu-id="27499-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27499-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="27499-127">Request body</span></span>
<span data-ttu-id="27499-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="27499-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27499-129">応答</span><span class="sxs-lookup"><span data-stu-id="27499-129">Response</span></span>
<span data-ttu-id="27499-130">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="27499-130">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27499-131">例</span><span class="sxs-lookup"><span data-stu-id="27499-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="27499-132">要求</span><span class="sxs-lookup"><span data-stu-id="27499-132">Request</span></span>
<span data-ttu-id="27499-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="27499-133">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="27499-134">応答</span><span class="sxs-lookup"><span data-stu-id="27499-134">Response</span></span>
<span data-ttu-id="27499-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="27499-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": [
    {
      "@odata.type": "microsoft.graph.managedAppDiagnosticStatus",
      "validationName": "Validation Name value",
      "state": "State value",
      "mitigationInstruction": "Mitigation Instruction value"
    }
  ]
}
```



