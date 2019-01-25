---
title: 連絡先を更新する
description: 連絡先オブジェクトのプロパティを更新します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c6ed3304b5f44a8bb1d35c1db491e8eaf7ae47b4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528208"
---
# <a name="update-contact"></a><span data-ttu-id="0d2d3-103">連絡先を更新する</span><span class="sxs-lookup"><span data-stu-id="0d2d3-103">Update contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d2d3-104">連絡先オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-104">Update the properties of contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0d2d3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0d2d3-105">Permissions</span></span>
<span data-ttu-id="0d2d3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d2d3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0d2d3-108">Permission type</span></span>      | <span data-ttu-id="0d2d3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0d2d3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d2d3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0d2d3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0d2d3-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d2d3-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0d2d3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0d2d3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d2d3-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d2d3-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0d2d3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0d2d3-114">Application</span></span> | <span data-ttu-id="0d2d3-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d2d3-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d2d3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0d2d3-116">HTTP request</span></span>
<span data-ttu-id="0d2d3-117"><!-- { "blockType": "ignored" } -->[連絡先](../resources/contact.md)ユーザーの既定の[contactFolder](../resources/contactfolder.md)からです。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-117"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="0d2d3-118">ユーザーの最上位レベル [contactFolder](../resources/contactfolder.md) からの [連絡先](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="0d2d3-119">[にお問い合わせください](../resources/contact.md) [contactFolder](../resources/mailfolder.md)の子フォルダーに含まれています。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-119">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="0d2d3-120">次の例は、入れ子のレベルを 1 つを示していますが、連絡先を子の子でというように配置できます。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-120">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0d2d3-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0d2d3-121">Request headers</span></span>
| <span data-ttu-id="0d2d3-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0d2d3-122">Header</span></span>       | <span data-ttu-id="0d2d3-123">値</span><span class="sxs-lookup"><span data-stu-id="0d2d3-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0d2d3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d2d3-124">Authorization</span></span>  | <span data-ttu-id="0d2d3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0d2d3-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0d2d3-127">Content-Type</span></span>  | <span data-ttu-id="0d2d3-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0d2d3-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0d2d3-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="0d2d3-130">Request body</span></span>
<span data-ttu-id="0d2d3-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0d2d3-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d2d3-134">Property</span></span>     | <span data-ttu-id="0d2d3-135">型</span><span class="sxs-lookup"><span data-stu-id="0d2d3-135">Type</span></span>   |<span data-ttu-id="0d2d3-136">説明</span><span class="sxs-lookup"><span data-stu-id="0d2d3-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d2d3-137">assistantName</span><span class="sxs-lookup"><span data-stu-id="0d2d3-137">assistantName</span></span>|<span data-ttu-id="0d2d3-138">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-138">String</span></span>|<span data-ttu-id="0d2d3-139">連絡先のアシスタントの名前。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-139">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="0d2d3-140">birthday</span><span class="sxs-lookup"><span data-stu-id="0d2d3-140">birthday</span></span>|<span data-ttu-id="0d2d3-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d2d3-141">DateTimeOffset</span></span>|<span data-ttu-id="0d2d3-142">連絡先の誕生日です。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-142">The contact's birthday.</span></span>|
|<span data-ttu-id="0d2d3-143">categories</span><span class="sxs-lookup"><span data-stu-id="0d2d3-143">categories</span></span>|<span data-ttu-id="0d2d3-144">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-144">String</span></span>|<span data-ttu-id="0d2d3-145">連絡先に関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-145">The categories associated with the contact.</span></span>|
|<span data-ttu-id="0d2d3-146">children</span><span class="sxs-lookup"><span data-stu-id="0d2d3-146">children</span></span>|<span data-ttu-id="0d2d3-147">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-147">String</span></span>||
|<span data-ttu-id="0d2d3-148">companyName</span><span class="sxs-lookup"><span data-stu-id="0d2d3-148">companyName</span></span>|<span data-ttu-id="0d2d3-149">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-149">String</span></span>|<span data-ttu-id="0d2d3-150">連絡先の会社の名前。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-150">The name of the contact's company.</span></span>|
|<span data-ttu-id="0d2d3-151">department</span><span class="sxs-lookup"><span data-stu-id="0d2d3-151">department</span></span>|<span data-ttu-id="0d2d3-152">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-152">String</span></span>|<span data-ttu-id="0d2d3-153">連絡先の部署。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-153">The contact's department.</span></span>|
|<span data-ttu-id="0d2d3-154">displayName</span><span class="sxs-lookup"><span data-stu-id="0d2d3-154">displayName</span></span>|<span data-ttu-id="0d2d3-155">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0d2d3-155">String</span></span>|<span data-ttu-id="0d2d3-156">連絡先の表示名。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-156">The contact's display name.</span></span> <span data-ttu-id="0d2d3-157">その他のプロパティを後で更新プログラムが原因で、自動的に生成された値を指定した表示名の値を上書きすることに注意します。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-157">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="0d2d3-158">既存の値を保持するには、必ず、更新操作の表示名としてです。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-158">To preserve a pre-existing value, always include it as displayName in an update operation.</span></span>|
|<span data-ttu-id="0d2d3-159">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="0d2d3-159">emailAddresses</span></span>|<span data-ttu-id="0d2d3-160">[typedEmailAddress](../resources/typedemailaddress.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0d2d3-160">[typedEmailAddress](../resources/typedemailaddress.md) collection</span></span>|<span data-ttu-id="0d2d3-161">連絡先のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-161">The contact's email addresses.</span></span>|
|<span data-ttu-id="0d2d3-162">fileAs</span><span class="sxs-lookup"><span data-stu-id="0d2d3-162">fileAs</span></span>|<span data-ttu-id="0d2d3-163">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-163">String</span></span>|<span data-ttu-id="0d2d3-164">連絡先がファイルされる名前。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-164">The name the contact is filed under.</span></span>|
|<span data-ttu-id="0d2d3-165">gender</span><span class="sxs-lookup"><span data-stu-id="0d2d3-165">gender</span></span> |<span data-ttu-id="0d2d3-166">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-166">String</span></span> |<span data-ttu-id="0d2d3-167">連絡先の性別。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-167">The contact's gender.</span></span> |
|<span data-ttu-id="0d2d3-168">generation</span><span class="sxs-lookup"><span data-stu-id="0d2d3-168">generation</span></span>|<span data-ttu-id="0d2d3-169">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-169">String</span></span>|<span data-ttu-id="0d2d3-170">連絡先の世代。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-170">The contact's generation.</span></span>|
|<span data-ttu-id="0d2d3-171">givenName</span><span class="sxs-lookup"><span data-stu-id="0d2d3-171">givenName</span></span>|<span data-ttu-id="0d2d3-172">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-172">String</span></span>|<span data-ttu-id="0d2d3-173">連絡先の名。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-173">The contact's given name.</span></span>|
|<span data-ttu-id="0d2d3-174">imAddresses</span><span class="sxs-lookup"><span data-stu-id="0d2d3-174">imAddresses</span></span>|<span data-ttu-id="0d2d3-175">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-175">String</span></span>|<span data-ttu-id="0d2d3-176">連絡先のインスタント メッセージング (IM) アドレス。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-176">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="0d2d3-177">initials</span><span class="sxs-lookup"><span data-stu-id="0d2d3-177">initials</span></span>|<span data-ttu-id="0d2d3-178">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-178">String</span></span>|<span data-ttu-id="0d2d3-179">連絡先のイニシャル。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-179">The contact's initials.</span></span>|
|<span data-ttu-id="0d2d3-180">jobTitle</span><span class="sxs-lookup"><span data-stu-id="0d2d3-180">jobTitle</span></span>|<span data-ttu-id="0d2d3-181">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-181">String</span></span>|<span data-ttu-id="0d2d3-182">連絡先の役職。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-182">The contact’s job title.</span></span>|
|<span data-ttu-id="0d2d3-183">manager</span><span class="sxs-lookup"><span data-stu-id="0d2d3-183">manager</span></span>|<span data-ttu-id="0d2d3-184">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-184">String</span></span>|<span data-ttu-id="0d2d3-185">連絡先の上司の名前。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-185">The name of the contact's manager.</span></span>
|<span data-ttu-id="0d2d3-186">middleName</span><span class="sxs-lookup"><span data-stu-id="0d2d3-186">middleName</span></span>|<span data-ttu-id="0d2d3-187">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-187">String</span></span>|<span data-ttu-id="0d2d3-188">連絡先のミドル ネーム。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-188">The contact's middle name.</span></span>|
|<span data-ttu-id="0d2d3-189">nickName</span><span class="sxs-lookup"><span data-stu-id="0d2d3-189">nickName</span></span>|<span data-ttu-id="0d2d3-190">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-190">String</span></span>|<span data-ttu-id="0d2d3-191">連絡先のニックネーム。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-191">The contact's nickname.</span></span>|
|<span data-ttu-id="0d2d3-192">officeLocation</span><span class="sxs-lookup"><span data-stu-id="0d2d3-192">officeLocation</span></span>|<span data-ttu-id="0d2d3-193">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-193">String</span></span>|<span data-ttu-id="0d2d3-194">連絡先のオフィスの所在地。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-194">The location of the contact's office.</span></span>|
|<span data-ttu-id="0d2d3-195">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="0d2d3-195">parentFolderId</span></span>|<span data-ttu-id="0d2d3-196">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-196">String</span></span>|<span data-ttu-id="0d2d3-197">連絡先の親フォルダーの ID。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-197">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="0d2d3-198">personalNotes</span><span class="sxs-lookup"><span data-stu-id="0d2d3-198">personalNotes</span></span>|<span data-ttu-id="0d2d3-199">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-199">String</span></span>|<span data-ttu-id="0d2d3-200">連絡先に関するユーザーのメモ。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-200">The user's notes about the contact.</span></span>|
|<span data-ttu-id="0d2d3-201">phones</span><span class="sxs-lookup"><span data-stu-id="0d2d3-201">phones</span></span> |<span data-ttu-id="0d2d3-202">[phone](../resources/phone.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0d2d3-202">[phone](../resources/phone.md) collection</span></span> |<span data-ttu-id="0d2d3-203">自宅電話、携帯電話、勤務先電話など、連絡先に関連付けられた電話番号。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-203">Phone numbers associated with the contact, for example, home phone, mobile phone, and business phone.</span></span> |
|<span data-ttu-id="0d2d3-204">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="0d2d3-204">postalAddresses</span></span> |<span data-ttu-id="0d2d3-205">[PhysicalAddress](../resources/physicaladdress.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0d2d3-205">[physicalAddress](../resources/physicaladdress.md) collection</span></span> |<span data-ttu-id="0d2d3-206">自宅住所や勤務先住所など、連絡先に関連付けられた住所。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-206">Addresses associated with the contact, for example, home address and business address.</span></span> |
|<span data-ttu-id="0d2d3-207">profession</span><span class="sxs-lookup"><span data-stu-id="0d2d3-207">profession</span></span>|<span data-ttu-id="0d2d3-208">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-208">String</span></span>|<span data-ttu-id="0d2d3-209">連絡先の専門的職業。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-209">The contact's profession.</span></span>|
|<span data-ttu-id="0d2d3-210">spouseName</span><span class="sxs-lookup"><span data-stu-id="0d2d3-210">spouseName</span></span>|<span data-ttu-id="0d2d3-211">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-211">String</span></span>|<span data-ttu-id="0d2d3-212">連絡先の配偶者/パートナーの名前。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-212">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="0d2d3-213">姓</span><span class="sxs-lookup"><span data-stu-id="0d2d3-213">surname</span></span>|<span data-ttu-id="0d2d3-214">文字列</span><span class="sxs-lookup"><span data-stu-id="0d2d3-214">String</span></span>|<span data-ttu-id="0d2d3-215">連絡先の姓。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-215">The contact's surname.</span></span>|
|<span data-ttu-id="0d2d3-216">タイトル</span><span class="sxs-lookup"><span data-stu-id="0d2d3-216">title</span></span>|<span data-ttu-id="0d2d3-217">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-217">String</span></span>|<span data-ttu-id="0d2d3-218">連絡先の肩書。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-218">The contact's title.</span></span>|
|<span data-ttu-id="0d2d3-219">websites</span><span class="sxs-lookup"><span data-stu-id="0d2d3-219">websites</span></span> |<span data-ttu-id="0d2d3-220">[website](../resources/website.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0d2d3-220">[website](../resources/website.md) collection</span></span>|<span data-ttu-id="0d2d3-221">連絡先に関連付けられた Web サイト。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-221">Web sites associated with the contact.</span></span> |
|<span data-ttu-id="0d2d3-222">WeddingAnniversary</span><span class="sxs-lookup"><span data-stu-id="0d2d3-222">weddingAnniversary</span></span> |<span data-ttu-id="0d2d3-223">日付</span><span class="sxs-lookup"><span data-stu-id="0d2d3-223">Date</span></span> |<span data-ttu-id="0d2d3-224">連絡先の結婚記念日。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-224">The contact's wedding anniversary.</span></span> |
|<span data-ttu-id="0d2d3-225">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="0d2d3-225">yomiCompanyName</span></span>|<span data-ttu-id="0d2d3-226">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-226">String</span></span>|<span data-ttu-id="0d2d3-p107">連絡先の会社名の読み仮名。このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-p107">The phonetic Japanese company name of the contact. This property is optional.</span></span>|
|<span data-ttu-id="0d2d3-229">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="0d2d3-229">yomiGivenName</span></span>|<span data-ttu-id="0d2d3-230">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-230">String</span></span>|<span data-ttu-id="0d2d3-p108">連絡先の名 (ファースト ネーム) の読み仮名。このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-p108">The phonetic Japanese given name (first name) of the contact. This property is optional.</span></span>|
|<span data-ttu-id="0d2d3-233">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="0d2d3-233">yomiSurname</span></span>|<span data-ttu-id="0d2d3-234">String</span><span class="sxs-lookup"><span data-stu-id="0d2d3-234">String</span></span>|<span data-ttu-id="0d2d3-p109">連絡先の姓 (ラスト ネーム) の読み仮名。このプロパティは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-p109">The phonetic Japanese surname (last name)  of the contact. This property is optional.</span></span>|

<span data-ttu-id="0d2d3-237">使用することができます**お問い合わせください**リソースは、[拡張機能](/graph/extensibility-overview)をサポートするため、`PATCH`を追加、更新、または既存の**連絡先**のインスタンスで拡張機能のカスタム プロパティに独自のアプリケーション固有データを削除する操作です。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-237">Since the **contact** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **contact** instance.</span></span>

## <a name="response"></a><span data-ttu-id="0d2d3-238">応答</span><span class="sxs-lookup"><span data-stu-id="0d2d3-238">Response</span></span>

<span data-ttu-id="0d2d3-239">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文のオブジェクトの更新に[お問い合わせください](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-239">If successful, this method returns a `200 OK` response code and updated [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0d2d3-240">例</span><span class="sxs-lookup"><span data-stu-id="0d2d3-240">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d2d3-241">要求</span><span class="sxs-lookup"><span data-stu-id="0d2d3-241">Request</span></span>
<span data-ttu-id="0d2d3-242">次の例では、指定した連絡先の個人用の電子メール アドレスを更新します。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-242">The following example updates the personal email address of the specified contact.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contact"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/contacts/AAMkADh6v5AAAvgTCEAAA=
Content-type: application/json

{
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@adatum.onmicrosoft.com"
        },
        {
          "address": "pavelb@fabrikam.onmicrosoft.com",
          "name": "Pavel Bansky",
          "type": "other",
          "otherLabel": "Volunteer work"
        }
    ]
}
```
##### <a name="response"></a><span data-ttu-id="0d2d3-243">応答</span><span class="sxs-lookup"><span data-stu-id="0d2d3-243">Response</span></span>
<span data-ttu-id="0d2d3-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0d2d3-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('c3e1fcd2-db78-42a8-aec5-1f2cd59abb5c')/contacts/$entity",
    "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fh\"",
    "id":"AAMkADh6v5AAAvgTCEAAA=",
    "createdDateTime":"2018-06-11T19:56:07Z",
    "lastModifiedDateTime":"2018-06-11T20:26:23Z",
    "changeKey":"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fh",
    "categories":[

    ],
    "parentFolderId":"AAMkADh6v5AAAAAAEOAAA=",
    "birthday":null,
    "fileAs":"",
    "displayName":"Pavel Bansky",
    "givenName":"Pavel",
    "initials":null,
    "middleName":null,
    "nickName":null,
    "surname":"Bansky",
    "title":null,
    "yomiGivenName":null,
    "yomiSurname":null,
    "yomiCompanyName":null,
    "generation":null,
    "imAddresses":[

    ],
    "jobTitle":null,
    "companyName":null,
    "department":null,
    "officeLocation":null,
    "profession":null,
    "assistantName":null,
    "manager":null,
    "spouseName":null,
    "personalNotes":"",
    "children":[

    ],
    "gender":null,
    "isFavorite":null,
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@adatum.onmicrosoft.com"
        },
        {
            "type":"other",
            "otherLabel":"Volunteer work",
            "name":"Pavel Bansky",
            "address":"pavelb@fabrikam.onmicrosoft.com"
        }
    ],
    "websites":[

    ],
    "phones":[
        {
            "type":"business",
            "number":"+1 732 555 0102"
        }
    ],
    "postalAddresses":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

## <a name="see-also"></a><span data-ttu-id="0d2d3-247">関連項目</span><span class="sxs-lookup"><span data-stu-id="0d2d3-247">See also</span></span>

- [<span data-ttu-id="0d2d3-248">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="0d2d3-248">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="0d2d3-249">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="0d2d3-249">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contact-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
