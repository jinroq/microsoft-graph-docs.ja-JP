---
title: employees リソースの種類
description: Dynamics 365 Business Central の employee オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 865da0c1e1256e2ba2a25902e37a00da9081eedf
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366656"
---
# <a name="employees-resource-type"></a><span data-ttu-id="29510-103">employees リソースの種類</span><span class="sxs-lookup"><span data-stu-id="29510-103">employees resource type</span></span>
<span data-ttu-id="29510-104">Dynamics 365 Business Central の従業員を表します。</span><span class="sxs-lookup"><span data-stu-id="29510-104">Represents an employee in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="29510-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="29510-105">Methods</span></span>

| <span data-ttu-id="29510-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="29510-106">Method</span></span>                                              | <span data-ttu-id="29510-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="29510-107">Return Type</span></span>|<span data-ttu-id="29510-108">説明</span><span class="sxs-lookup"><span data-stu-id="29510-108">Description</span></span>               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[<span data-ttu-id="29510-109">従業員の取得</span><span class="sxs-lookup"><span data-stu-id="29510-109">Get employees</span></span>](../api/dynamics-employee-get.md)      |<span data-ttu-id="29510-110">向け</span><span class="sxs-lookup"><span data-stu-id="29510-110">employees</span></span>  |<span data-ttu-id="29510-111">employee オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="29510-111">Get an employee object.</span></span>   |
|[<span data-ttu-id="29510-112">従業員の投稿</span><span class="sxs-lookup"><span data-stu-id="29510-112">Post employees</span></span>](../api/dynamics-create-employee.md)  |<span data-ttu-id="29510-113">向け</span><span class="sxs-lookup"><span data-stu-id="29510-113">employees</span></span>  |<span data-ttu-id="29510-114">employee オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="29510-114">Create an employee object.</span></span>|
|[<span data-ttu-id="29510-115">パッチの従業員</span><span class="sxs-lookup"><span data-stu-id="29510-115">Patch employees</span></span>](../api/dynamics-employee-update.md) |<span data-ttu-id="29510-116">向け</span><span class="sxs-lookup"><span data-stu-id="29510-116">employees</span></span>  |<span data-ttu-id="29510-117">employee オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="29510-117">Update an employee object.</span></span>|
|[<span data-ttu-id="29510-118">従業員を削除する</span><span class="sxs-lookup"><span data-stu-id="29510-118">Delete employees</span></span>](../api/dynamics-employee-delete.md)|<span data-ttu-id="29510-119">none</span><span class="sxs-lookup"><span data-stu-id="29510-119">none</span></span>       |<span data-ttu-id="29510-120">employee オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="29510-120">Delete an employee object.</span></span>|

## <a name="properties"></a><span data-ttu-id="29510-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29510-121">Properties</span></span>
| <span data-ttu-id="29510-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29510-122">Property</span></span>           | <span data-ttu-id="29510-123">型</span><span class="sxs-lookup"><span data-stu-id="29510-123">Type</span></span>   |<span data-ttu-id="29510-124">説明</span><span class="sxs-lookup"><span data-stu-id="29510-124">Description</span></span>                                            |
|:-------------------|:-------|:------------------------------------------------------|
|<span data-ttu-id="29510-125">ID</span><span class="sxs-lookup"><span data-stu-id="29510-125">id</span></span>                  |<span data-ttu-id="29510-126">GUID</span><span class="sxs-lookup"><span data-stu-id="29510-126">GUID</span></span>    |<span data-ttu-id="29510-127">従業員 ID。</span><span class="sxs-lookup"><span data-stu-id="29510-127">The employee ID.</span></span> <span data-ttu-id="29510-128">編集不可。</span><span class="sxs-lookup"><span data-stu-id="29510-128">Non-editable.</span></span>                         |
|<span data-ttu-id="29510-129">number</span><span class="sxs-lookup"><span data-stu-id="29510-129">number</span></span>              |<span data-ttu-id="29510-130">string</span><span class="sxs-lookup"><span data-stu-id="29510-130">string</span></span>  |<span data-ttu-id="29510-131">従業員番号。</span><span class="sxs-lookup"><span data-stu-id="29510-131">The employee number.</span></span> <span data-ttu-id="29510-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="29510-132">Read-Only.</span></span>                        |
|<span data-ttu-id="29510-133">displayName</span><span class="sxs-lookup"><span data-stu-id="29510-133">displayName</span></span>         |<span data-ttu-id="29510-134">string</span><span class="sxs-lookup"><span data-stu-id="29510-134">string</span></span>  |<span data-ttu-id="29510-135">従業員の givenName + 姓。</span><span class="sxs-lookup"><span data-stu-id="29510-135">The employee givenName + surname.</span></span> <span data-ttu-id="29510-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="29510-136">Read-Only.</span></span>           |
|<span data-ttu-id="29510-137">givenName</span><span class="sxs-lookup"><span data-stu-id="29510-137">givenName</span></span>           |<span data-ttu-id="29510-138">string</span><span class="sxs-lookup"><span data-stu-id="29510-138">string</span></span>  |<span data-ttu-id="29510-139">従業員の指定された名前。</span><span class="sxs-lookup"><span data-stu-id="29510-139">The given name of the employee.</span></span>                        |
|<span data-ttu-id="29510-140">middleName</span><span class="sxs-lookup"><span data-stu-id="29510-140">middleName</span></span>          |<span data-ttu-id="29510-141">string</span><span class="sxs-lookup"><span data-stu-id="29510-141">string</span></span>  |<span data-ttu-id="29510-142">従業員のミドルネーム。</span><span class="sxs-lookup"><span data-stu-id="29510-142">The middle name of the employee.</span></span>                       |
|<span data-ttu-id="29510-143">surname</span><span class="sxs-lookup"><span data-stu-id="29510-143">surname</span></span>             |<span data-ttu-id="29510-144">string</span><span class="sxs-lookup"><span data-stu-id="29510-144">string</span></span>  |<span data-ttu-id="29510-145">従業員の姓</span><span class="sxs-lookup"><span data-stu-id="29510-145">The surname of the employee</span></span>                            |
|<span data-ttu-id="29510-146">jobTitle</span><span class="sxs-lookup"><span data-stu-id="29510-146">jobTitle</span></span>            |<span data-ttu-id="29510-147">string</span><span class="sxs-lookup"><span data-stu-id="29510-147">string</span></span>  |<span data-ttu-id="29510-148">従業員の正式な名前</span><span class="sxs-lookup"><span data-stu-id="29510-148">The full name of the employee</span></span>                          |
|<span data-ttu-id="29510-149">address</span><span class="sxs-lookup"><span data-stu-id="29510-149">address</span></span>             |[<span data-ttu-id="29510-150">ナビゲーション."postaladdress</span><span class="sxs-lookup"><span data-stu-id="29510-150">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="29510-151">従業員の住所を指定します。</span><span class="sxs-lookup"><span data-stu-id="29510-151">Specifies the employee's address.</span></span> <span data-ttu-id="29510-152">このアドレスは、従業員のすべてのリソースドキュメントに表示されます。</span><span class="sxs-lookup"><span data-stu-id="29510-152">This address will appear on all resource documents for the employee.</span></span>|
|<span data-ttu-id="29510-153">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="29510-153">phoneNumber</span></span>         |<span data-ttu-id="29510-154">string</span><span class="sxs-lookup"><span data-stu-id="29510-154">string</span></span>  |<span data-ttu-id="29510-155">従業員の電話番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="29510-155">Specifies the employee's telephone number.</span></span>             |
|<span data-ttu-id="29510-156">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="29510-156">mobilePhone</span></span>         |<span data-ttu-id="29510-157">string</span><span class="sxs-lookup"><span data-stu-id="29510-157">string</span></span>  |<span data-ttu-id="29510-158">従業員の携帯電話番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="29510-158">Specifies the employee's mobile telephone number.</span></span>      |
|<span data-ttu-id="29510-159">email</span><span class="sxs-lookup"><span data-stu-id="29510-159">email</span></span>               |<span data-ttu-id="29510-160">string</span><span class="sxs-lookup"><span data-stu-id="29510-160">string</span></span>  |<span data-ttu-id="29510-161">従業員の電子メールアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="29510-161">Specifies the employee's email address.</span></span>                |
|<span data-ttu-id="29510-162">パーソナル電子メール</span><span class="sxs-lookup"><span data-stu-id="29510-162">personalEmail</span></span>       |<span data-ttu-id="29510-163">string</span><span class="sxs-lookup"><span data-stu-id="29510-163">string</span></span>  |<span data-ttu-id="29510-164">従業員の個人の電子メールアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="29510-164">Specifies the employee's personal email address.</span></span>       |
|<span data-ttu-id="29510-165">employmentDate</span><span class="sxs-lookup"><span data-stu-id="29510-165">employmentDate</span></span>      |<span data-ttu-id="29510-166">日付</span><span class="sxs-lookup"><span data-stu-id="29510-166">date</span></span>    |<span data-ttu-id="29510-167">従業員が会社の作業を開始した日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="29510-167">Specifies the date when the employee began to work for the company.</span></span>|
|<span data-ttu-id="29510-168">終了した日付</span><span class="sxs-lookup"><span data-stu-id="29510-168">terminationDate</span></span>     |<span data-ttu-id="29510-169">日付</span><span class="sxs-lookup"><span data-stu-id="29510-169">date</span></span>    |<span data-ttu-id="29510-170">退職または棄却のために従業員が終了した日付を指定します (例:)。</span><span class="sxs-lookup"><span data-stu-id="29510-170">Specifies the date when the employee was terminated, due to retirement or dismissal, for example.</span></span>|
|<span data-ttu-id="29510-171">status</span><span class="sxs-lookup"><span data-stu-id="29510-171">status</span></span>              |<span data-ttu-id="29510-172">string</span><span class="sxs-lookup"><span data-stu-id="29510-172">string</span></span>  |<span data-ttu-id="29510-173">従業員の状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="29510-173">Specifies the employee's status.</span></span> <span data-ttu-id="29510-174">有効な値、非アクティブな値、または終了した値を指定します。</span><span class="sxs-lookup"><span data-stu-id="29510-174">Possible values are Active, Inactive or Terminated</span></span>|
|<span data-ttu-id="29510-175">birthDate</span><span class="sxs-lookup"><span data-stu-id="29510-175">birthDate</span></span>           |<span data-ttu-id="29510-176">日付</span><span class="sxs-lookup"><span data-stu-id="29510-176">date</span></span>    |<span data-ttu-id="29510-177">従業員の生年月日を指定します。</span><span class="sxs-lookup"><span data-stu-id="29510-177">Specifies the employee's date of birth.</span></span>                |
|<span data-ttu-id="29510-178">表</span><span class="sxs-lookup"><span data-stu-id="29510-178">picture</span></span>             |<span data-ttu-id="29510-179">stream</span><span class="sxs-lookup"><span data-stu-id="29510-179">stream</span></span>  |<span data-ttu-id="29510-180">従業員の画像。</span><span class="sxs-lookup"><span data-stu-id="29510-180">The employee picture.</span></span> <span data-ttu-id="29510-181">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="29510-181">Read-Only.</span></span>                       |
|<span data-ttu-id="29510-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29510-182">lastModifiedDateTime</span></span>|<span data-ttu-id="29510-183">datetime</span><span class="sxs-lookup"><span data-stu-id="29510-183">datetime</span></span>|<span data-ttu-id="29510-184">従業員が最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="29510-184">The last datetime the employee was modified.</span></span> <span data-ttu-id="29510-185">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="29510-185">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="29510-186">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="29510-186">Relationships</span></span>
<span data-ttu-id="29510-187">なし</span><span class="sxs-lookup"><span data-stu-id="29510-187">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29510-188">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="29510-188">JSON representation</span></span>

<span data-ttu-id="29510-189">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="29510-189">Here is a JSON representation of the resource.</span></span>


```json
{
    "id": "GUID",
    "number": "string",
    "displayName": "string",
    "givenName": "string",
    "middleName": "string",
    "surname": "string",
    "jobTitle": "string",
    "address": "NAV.PostalAddress",
    "phoneNumber": "string",
    "mobilePhone": "string",
    "email": "string",
    "personalEmail": "string",
    "employmentDate": "date",
    "terminationDate": "date",
    "status": "string",
    "birthDate": "date",
    "picture": "stream",
    "lastModifiedDateTime": "datetime"
}

```

