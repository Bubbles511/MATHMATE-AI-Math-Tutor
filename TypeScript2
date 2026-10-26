import { jsonb, pgTable, text, timestamp } from "drizzle-orm/pg-core";

export const studentStateTable = pgTable("mathmate_student_state", {
  userId: text("user_id").primaryKey(),
  state: jsonb("state").$type<Record<string, unknown>>().notNull(),
  updatedAt: timestamp("updated_at", { withTimezone: true }).notNull().defaultNow(),
});
